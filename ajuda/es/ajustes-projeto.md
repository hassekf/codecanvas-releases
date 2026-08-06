---
slug: ajustes-projeto
titulo: Ajustes del proyecto
resumo: La ventana del canvas: la máquina donde vive, la carpeta en la que nacen los agentes, el nombre, y las demás secciones.
area: projeto
nivel: basico
---

Abre el selector de proyecto, a la izquierda de la barra de comandos, y elige **Editar “nombre del
proyecto”…**. En la pantalla inicial, lo mismo se alcanza con el **⋯** de la esquina de la tarjeta o
con el clic derecho en ella.

La ventana tiene un menú lateral, y la primera sección es **Proyecto**.

## Dónde vive este proyecto

- **En esta máquina**: la carpeta es una carpeta de tu Mac.
- **En un servidor mío**: el proyecto y sus agentes viven en otra máquina, que sigue trabajando con
  el Mac apagado. Elegido esto, el control de la carpeta local desaparece. Ver
  [canvas remoto](canvas-remoto).

## Carpeta del proyecto

Todo agente de este canvas nace en esta carpeta, y es la carpeta que ven el Git, los archivos y el
navegador de los agentes. El botón **Elegir…** abre el selector de carpetas de macOS.

Cambiar la carpeta con agentes en pie:

- Un aviso aparece en la propia sección, antes de que guardes, diciendo cuántos agentes están
  corriendo en la carpeta antigua.
- Al guardar, la app pregunta qué hacer con ellos. **Reabrir con la conversación** cierra y recrea
  cada agente en la carpeta nueva llevándose su conversación: vuelve recordándolo todo, pero lo que
  estaba haciendo en ese instante se pierde. **Dejar en la carpeta antigua** mantiene los procesos
  vivos donde están, y solo los próximos agentes nacen en la carpeta nueva.
- Cuando algún agente no pueda llevarse la conversación, la app dice cuáles son, por su nombre, y
  cuántos vuelven enteros, antes de tocar nada. Desde ahí puedes reabrir de todos modos o cancelar.
  La conversación antigua no se borra en ninguno de los dos casos.

## Nombre

Es por el que llamas al proyecto en el selector, en la pantalla inicial y por voz. En blanco, al
crear, la app usa el nombre de la carpeta.

## Cambiar la cuenta del proyecto

Si la cuenta en la que nacen los agentes cambia y hay agentes vivos que la heredan, la app pregunta
qué hacer con su conversación: **Llevar las conversaciones** copia el pasado de cada uno dentro de
la carpeta de la cuenta nueva, y **Empezar de cero en la cuenta nueva** deja ese pasado donde está.
No se borra nada de la cuenta antigua, y quien eligió su propia cuenta en el menú del panel no se ve
afectado. Ver [cuentas y perfiles](contas-e-perfis).

## Las demás secciones

- **Agentes**: la instalación de Claude en la que nacen los agentes de este proyecto, las flags con
  las que nacen, si abren páginas en el navegador interno o en el externo, y el aislamiento por
  worktree. Ver [cuentas y perfiles](contas-e-perfis) y
  [worktrees y aislamiento](worktrees-e-isolamento).
- **Skills**: las capacidades que pueden usar los agentes de aquí. Ver
  [ajustes de skills](ajustes-skills).
- **MCP**: los servidores de herramientas que levantan los agentes de aquí. Ver
  [ajustes de MCP](ajustes-mcp).
- **Navegador**: la página en la que abre un navegador nuevo. Ver
  [ajustes del navegador](ajustes-navegador).
- **Apariencia**: el tema, la fuente de la interfaz y el fondo de este canvas, más el contorno del
  panel seleccionado, que vale para todos los canvases. Ver
  [apariencia del proyecto](ajustes-aparencia).
- **Anuncios**: las alertas que los agentes disparan en tu pantalla al cumplir una regla tuya. Ver
  [anuncios](ajustes-anuncios).
- **Integraciones**: las conexiones de este proyecto, como el Jira. Ver
  [integraciones](ajustes-integracoes).

Al **crear** un canvas, Skills, Anuncios e Integraciones no aparecen en el menú lateral: las tres
necesitan un proyecto que ya exista. Aparecen en cuanto guardas.

## La vista previa de la apariencia

Mientras esta ventana está abierta, tocar el tema, el fondo de pantalla o la oscuridad del velo
cambia el lienzo de detrás al instante. Solo el botón **Guardar** graba la elección: **Cancelar**,
Esc y el clic fuera devuelven la apariencia que estaba antes.

## Esto no es lo mismo que Ajustes

**⌘,** abre los ajustes de la app: la voz, el micrófono, los atajos, la escala de la interfaz, la
fuente de las terminales, el ancho máximo de un panel, las notificaciones. Todo eso vale para todos
los proyectos. Lo que editas en esta ventana vale solo para este canvas.
