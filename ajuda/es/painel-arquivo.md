---
slug: painel-arquivo
titulo: El panel de archivo
resumo: Leer un archivo del proyecto en un panel, editarlo cuando aparece el lápiz, y qué pasa cuando el disco cambia por debajo.
area: paineis
nivel: basico
---

Un archivo del proyecto abierto en un panel del lienzo.

## Abrir

- **Desde el cajón de archivos**, en el pie: dos clics en un archivo lo abren.
- **Con `⌘K`**, escribiendo el nombre del archivo.
- **Por un agente**, cuando quiere mostrarte algo.
- **Por voz**: *"muéstrame el README"*.

Un archivo ya abierto no genera un segundo panel: el que existe se trae al frente.

## El cajón de archivos

- **El campo de arriba** filtra el árbol por nombre.
- **Un clic** en un archivo lo adjunta al próximo prompt que envíes. La franja debajo del árbol dice
  cuál está adjunto, y su **×** deshace el adjunto.
- **Dos clics** abren el archivo en un panel.
- **El ojo de arriba** muestra y esconde los archivos que empiezan con punto. La elección vale para
  todos los proyectos, y el árbol se rehace solo al cambiarla.
- **Clic derecho**: **Abrir para leer**, **Copiar ruta**, **Copiar ruta relativa**, **Enviar a…** (a
  un agente de este lienzo, sin pasar por el portapapeles) y **Mostrar en Finder**.

## Qué muestra el panel

- **Markdown** viene renderizado. El botón de la cabecera alterna entre el fuente y el texto
  renderizado, y solo existe en archivos de Markdown.
- **Código** viene con numeración de línea y resaltado de sintaxis.
- **Una imagen** aparece ajustada al panel. Hacer clic alterna entre ajustada y tamaño real, y el
  pie muestra las dimensiones en píxeles. El clic derecho ofrece **Copiar imagen** (el contenido, no
  la ruta), **Copiar ruta** y **Mostrar en Finder**.
- **El video** se reproduce con los controles del sistema.
- **Un archivo binario** se declara como tal, con su tamaño.
- **Un archivo que ya no existe** lo dice en lugar del contenido.

El panel se recarga solo cuando el archivo cambia en el disco, incluidas las imágenes regeneradas
por un agente.

## Los botones de la cabecera

- **Editar** (el lápiz): entra en modo de edición. Aparece solo en texto y Markdown, con el archivo
  grabable, entero y de hasta 1 MB.
- **Copiar la ruta completa**: pone la ruta absoluta en el portapapeles.
- **Mostrar en Finder**: selecciona el archivo en el Finder.

El clic derecho, tanto en la cabecera como en el contenido, trae **Copiar la ruta completa**,
**Enviar a un agente** y **Enviar a un contacto**. Los agentes de este lienzo aparecen directo; los
de otros proyectos quedan en submenús, y enviar allá no cambia tu lienzo.

## Editar

- **Guardar** (`⌘S` o el botón): graba en el disco. No hay guardado automático. La tecla vale para
  el panel seleccionado, que es lo que decide qué archivo se graba cuando hay dos en edición.
- **Revertir a lo guardado**: devuelve el texto a lo que está en el disco, sin salir de la edición.
  No disponible cuando no hay cambio pendiente.
- **Salir de la edición**: con un cambio pendiente, pregunta antes de descartar, con **Descartar** y
  **Seguir editando**.
- **El punto junto al nombre del archivo** indica que hay un cambio sin guardar.

Un archivo cortado por tamaño no se puede editar, porque grabarlo de vuelta grabaría el corte. La
lectura corta en 4 MB, con el aviso al final del texto.

## Cuando el disco cambia por debajo de tu edición

Aparece una franja en cuanto el archivo cambia en el disco mientras hay una edición sin guardar,
diciendo el nombre de quien lo tocó cuando es identificable. Ella **impide el guardado** hasta que
elijas:

- **Recargar**: descarta lo que escribiste y trae lo que está en el disco.
- **Sobrescribir**: graba tu texto sobre el cambio del disco.

Fuera del modo de edición, el panel solo acompaña el disco, sin ninguna franja.

Guardar te registra como autor de ese archivo, y el [panel de Git](painel-git) pasa a
marcar disputa entre tú y un agente.
