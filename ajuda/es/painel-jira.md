---
slug: painel-jira
titulo: El panel de Jira
resumo: El tablero del proyecto conectado dentro del lienzo: filtros, arrastrar tarjetas, detalle de la incidencia y el camino hasta un agente.
area: paineis
nivel: basico
---

Ábrelo con `⌘K` y **jira**, **board**, **cuadro**, **issues**, **sprint**, **atlassian**, **tickets**
o **incidencias**. El panel solo muestra el tablero en un lienzo conectado; la conexión se hace en
[Jira y Confluence](jira-e-confluence).

Las columnas son las del tablero configurado en Jira, en el mismo orden. Un proyecto sin tablero de
software cae en las categorías de estado de Jira.

## La barra del panel

- **El nombre de arriba**: el nombre del sitio Atlassian de la conexión, no el del lienzo.
- **La clave del proyecto**, al lado del nombre: abre la lista de proyectos que alcanzan las
  credenciales de este lienzo y cambia el proyecto del panel. No disponible cuando las credenciales
  alcanzan un solo proyecto.
- **Actualizar**: recarga el tablero.
- **Nueva incidencia**: abre la creación de una incidencia. No disponible mientras no haya un
  proyecto elegido.

## Filtros y búsqueda

- **Todos**, **Míos**, **Bugs**: filtran las tarjetas. **Míos** compara con el nombre de la cuenta
  conectada; **Bugs** compara con el tipo de la incidencia.
- **Responsable**: filtra por una persona, entre las que aparecen en el tablero. Elegir a alguien
  estando en **Míos** devuelve el filtro a **Todos**, y elegir **Míos** limpia el responsable: los
  dos se anularían.
- **Mostrar etiquetas** y **Ocultar etiquetas**: muestran las etiquetas en las tarjetas. La elección
  vale para todos los lienzos y sobrevive al cerrar la app.
- **Buscar**: coincide con el título y con la clave de la incidencia.

El filtro rápido y el responsable quedan guardados en la conexión del lienzo y vuelven cuando
reabres el panel. La búsqueda no: se va con el panel.

Todas las columnas siguen visibles aunque un filtro vacíe alguna. El número al lado del nombre de la
columna cuenta las tarjetas visibles en ella.

## Mover y reordenar

- **Arrastrar una tarjeta a otra columna**: cambia el estado en Jira. Si el cambio es rechazado, la
  tarjeta vuelve a su sitio y aparece un aviso al pie del panel durante unos segundos.
- **Soltar una tarjeta sobre otra de la misma columna**: reordena las dos en Jira. Entre columnas
  distintas, el mismo gesto vale como cambio de estado.

## La tarjeta

- **Hacer clic**: abre el detalle de la incidencia.
- **Abrir detalles**, en el menú **⋯**: el mismo detalle.
- **Enviar a un agente**, en el menú **⋯**: solo aparece con algún agente abierto en el lienzo.
- **Copiar la clave**, en el menú **⋯**: copia la clave de la incidencia.
- **Arrastrar la tarjeta dentro de un panel de agente**: escribe la clave y el título en su campo,
  **sin** enviarlo, y pone el agente en foco. Tú completas la frase y envías. A partir de la clave el
  agente lee la incidencia entera por su cuenta.

## El detalle de la incidencia

- **Estado**: se vuelve un menú con las transiciones que Jira permite ahí. Sin permiso de transición
  es solo un campo de lectura.
- **El lápiz**: edita el título y la descripción. Solo aparece con permiso de edición. La descripción
  solo se reenvía a Jira si la tocas, para que el formato original no se pierda al guardar solo el
  título.
- **Adjuntar**: envía un archivo a la incidencia.
- **Comentar**: `Enter` envía, `Shift+Enter` salta de línea. El campo solo existe con permiso de
  comentar.
- **Una imagen adjunta o incrustada en un comentario**: al hacer clic se amplía; ampliada, **Enviar
  al lienzo** la pega en el lienzo.
- **Un enlace en la descripción o en un comentario**: pregunta entre **Abrir aquí**, que abre un
  panel de navegador de este lienzo, y **En el navegador externo**.
- **Enviar a un agente**, al pie: manda la mención y cierra el detalle.
- **Copiar la clave** y **Abrir en Jira**, al pie: la clave al portapapeles, y la página de la
  incidencia en tu navegador.

Cambiar el estado, comentar y editar aparecen en la pantalla antes de que Jira confirme. Si la
llamada falla, el valor anterior vuelve y un aviso cuenta lo que pasó.

## Nueva incidencia

- **Espacio**: el sitio y el proyecto de este lienzo, ya elegidos.
- **Tipo de ticket**: los tipos que el proyecto acepta, cargados de Jira al abrir.
- **Estado**: la columna en la que nace la incidencia. La app la crea y después intenta moverla allí;
  sin transición disponible, se queda donde nació.
- **Resumen**: obligatorio.
- **Descripción**: opcional.

Creada, la tarjeta sube al principio de la columna.

## Cuando el panel no tiene qué mostrar

- **Sin conexión**: el botón **Conectar Jira** abre la edición de este workspace en la parte de
  Atlassian.
- **Sin proyecto elegido**: el botón **Elegir el proyecto** lleva al mismo sitio.
- **Proyecto sin incidencias**: el panel lo dice, y **Nueva incidencia** sigue disponible.

## Configurado en otra pantalla

- La conexión, el proyecto y los avisos de Jira: [Jira y Confluence](jira-e-confluence).
- El acceso directo a la conexión, dentro de Configuración: [Integraciones](ajustes-integracoes).
