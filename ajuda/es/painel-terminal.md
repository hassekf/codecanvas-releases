---
slug: painel-terminal
titulo: El panel de terminal
resumo: Una shell en la carpeta del proyecto, dentro del lienzo: cómo abrirla, qué hacen los gestos, y de dónde vienen la fuente y el nombre.
area: paineis
nivel: basico
---

Una shell del sistema ejecutándose en la carpeta del proyecto de este lienzo, sin ningún agente
encima.

## Abrir y cerrar

- **`⌘K`, escribiendo "terminal"**: abre un panel nuevo. Cada llamada abre uno más, a diferencia del
  [panel de Git](painel-git) y del [panel del elenco](painel-elenco), que son uno por lienzo.
- **`⌘T`**: lo mismo, sin pasar por la [búsqueda](busca-e-comandos). La tecla se cambia en
  Ajustes → Atajos.
- **Cerrar el panel termina el proceso.** Cambiar de lienzo no: la shell sigue corriendo fuera de
  vista, y el panel vuelve con lo que imprimió mientras estabas en otro proyecto.

## El nombre del panel

- **Doble clic en el título**: abre el campo de edición. Enter confirma, Esc cancela, y hacer clic
  fuera también confirma.
- **El terminal es el único panel con nombre editable.** Un agente ya tiene nombre propio, y los
  demás paneles derivan el título de lo que muestran.
- **El nombre es una dirección.** Es por él que la [búsqueda](busca-e-comandos), Nina y los agentes
  encuentran el panel: un terminal llamado "deploy" pasa a responder a "deploy" en los tres.

## Gestos dentro del terminal

- **Clic en una ruta impresa**: la app busca el archivo en el disco y lo abre donde mejor se lee, un
  [panel de archivo](painel-arquivo) para texto, el navegador para una página, el Finder para lo
  demás. Las rutas relativas se cuentan desde la carpeta en la que está este terminal. Si no
  encuentra nada, la app lo avisa en vez de abrir una ventana vacía.
- **Clic en una dirección web**: abre en un [panel de navegador](painel-navegador), o en el
  navegador del sistema si este lienzo está configurado para el externo, en la pestaña **Agentes**
  de los [ajustes del proyecto](ajustes-projeto).
- **Arrastrar archivos del Finder dentro**: escribe las rutas, escapadas, en la línea de comandos.
  No se ejecuta nada, y ningún agente interviene.

## La letra

- **El zoom del lienzo cambia el tamaño de la fuente**, no la escala de la imagen. El número de
  columnas se mantiene prácticamente igual en cualquier zoom, y el texto no se reajusta al acercar o
  alejar.
- **Fuente y tamaño de partida**: Ajustes → Terminal. Solo se ofrecen fuentes monoespaciadas, y la
  elección vale para todos los terminales y agentes de la app, incluidos los que están fuera de
  vista.

## Comandos que no terminan

Un agente que ejecuta un servidor de desarrollo, un observador de archivos o cualquier comando que
no retorna se queda atrapado en él. La app desvía esos comandos a un panel de terminal propio,
visible en el lienzo, y le avisa al agente del desvío. Los comandos que terminan pasan directo.

Ese es el ajuste **Dev servers en su propio panel**, en Ajustes → Agentes. Desactivado, el agente
ejecuta todo dentro de sí, y un servidor de desarrollo le bloquea la conversación sin aparecer en
ningún lado. Más en [hablar con ellos](falar-com-eles).
