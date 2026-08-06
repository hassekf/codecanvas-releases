---
slug: os-paineis-e-a-mesa
titulo: Los paneles y la mesa
resumo: Abrir, mover, redimensionar, seleccionar y cerrar paneles, y los dos modos en que la mesa se ordena.
area: canvas
nivel: basico
---

## Abrir un panel

- **⌘K** y el nombre de lo que quieres: terminal, navegador, git, notas. Ver
  [búsqueda y comandos](busca-e-comandos).
- **Los botones de la barra de comandos**, abajo: **Buscar en el lienzo**, **Nuevo agente** y
  **Nuevo navegador**.
- **⌘N** abre un agente, **⌘⇧N** abre un agente de Codex (solo con Codex activado en
  **Ajustes → Proveedores**) y **⌘T** abre una terminal sin agente encima. Los tres funcionan
  incluso con el cursor dentro de otro agente.
- **Por voz**: *"abre un navegador"*, *"abre el git"*.

Los agentes también abren paneles por su cuenta. Ver
[el agente toca el lienzo](o-agente-mexe-no-canvas).

## La cabecera

Arrastrar por la cabecera mueve el panel. Hacer clic en ella trae el panel al frente y lo selecciona.

- **El botón de soltar**: saca el panel de la disposición automática y le da posición y tamaño
  propios, sobre la cuadrícula. Solo existe en la cuadrícula automática, y un panel suelto no puede
  estar destacado al mismo tiempo.
- **El botón de destacar**: pone este panel grande a la izquierda y apila los demás en una columna a
  la derecha. No aparece en un panel suelto. Por voz, *"foco en Perseu"* y *"quita el foco"* hacen
  lo mismo.
- **Minimizar**: guarda el panel en el [estante](minimizar-e-a-estante), con el contenido vivo.
- **Cerrar**: saca el panel del lienzo. Un agente cerrado se despide, no se borra: ver
  [crear y cerrar](criar-e-fechar).

El clic derecho en la cabecera abre el menú del panel: escribir un asunto fijo para él, cambiar la
cuenta del agente, minimizar, y **Mover al área**, que solo aparece cuando el proyecto tiene más de
un [área de trabajo](areas-de-trabalho).

## Los dos modos de la mesa

El selector está en la barra de comandos, y la elección es **de cada área de trabajo**: la
cuadrícula del front no toca la del back.

- **Cuadrícula automática**: la app decide la posición y el tamaño de todos. Abrir o cerrar un panel
  redistribuye a los demás al instante. Arrastrar un panel y soltarlo cerca de otro intercambia los
  dos, dentro de la misma área.
- **Lienzo libre**: la posición y el tamaño son tuyos. Arrastra por la cabecera para mover, y tira
  de cualquiera de los cuatro lados o de las cuatro esquinas para redimensionar. El cursor cambia al
  acercarse al borde.

Volver a la cuadrícula automática deshace la disposición que montaste a mano. El aviso que aparece
en ese cambio trae **Deshacer**.

## Elegir la disposición de la cuadrícula

El minimapa está en la esquina inferior derecha. Aparece en cada cambio de disposición y se recoge
en un icono tras un instante, volviendo cuando el cursor se acerca. Al hacer clic, eliges entre las
disposiciones posibles para la cantidad de paneles abiertos: la automática, desde una sola columna
hasta una columna por panel, y la de destaque.

## Alinear a la cuadrícula

El botón **Alinear a la cuadrícula** aparece en la barra de comandos **solo en el lienzo libre**.
Con él activado, lo que mueves y redimensionas encaja de 40 en 40 puntos. Al arrastrar solo se
alinea la posición; al redimensionar, también el tamaño. Es una preferencia de tu pantalla: vale
para todos los proyectos.

## Seleccionar

- **Clic**: selecciona un panel y lo trae al frente.
- **⌘ con clic**: añade a la selección, o saca de ella lo que ya estaba marcado.
- **Arrastre con el botón izquierdo sobre un área vacía**: dibuja un lazo que atrapa todo lo que
  toca, no solo lo que cabe entero dentro. La selección ocurre durante el arrastre.
- **Clic en un área vacía**: limpia la selección.

Arrastrar un panel que ya está seleccionado se lleva **todos** los seleccionados.

El color, el grosor y el brillo del contorno están en el bloque **Panel seleccionado**, en la
sección [Apariencia](ajustes-aparencia) del editor del proyecto. Esa elección vale para todos los
canvases.

## Cerrar

- **La ✕ de la cabecera** cierra ese panel.
- **Delete** cierra los paneles seleccionados **a partir de dos**. Con un solo panel seleccionado, la
  tecla no hace nada. Con imágenes del lienzo seleccionadas, borra las imágenes en vez de los
  paneles. Y nunca se dispara mientras escribes en una terminal o en un campo de texto. La tecla se
  configura en **Ajustes → Atajos**.
- **Por voz**: *"cierra los agentes"*, *"cierra dos navegadores"*, *"cierra a Juno y a Diana"*,
  *"cierra todo"*. Cerrar por tipo y *"todo"* actúan solo sobre el área de trabajo abierta; por
  nombre, alcanza a un panel de cualquier área. Si algún objetivo está trabajando, la app devuelve
  la pregunta en vez de cerrar, y empieza por los que están parados cuando tiene que elegir cuántos.

## Ancho máximo de un panel

En **Ajustes → Interfaz**, el control **Ancho máximo de un panel** va de 600 a 4000 px, con 1500 px
de fábrica. Limita un panel que está **solo** en pantalla, que queda centrado; varios paneles siguen
usando toda la pantalla. Solo tiene efecto en la cuadrícula automática, y vale para todos los
proyectos. Por voz: *"ancho máximo 1500"*.

## Juntar agentes en un solo panel

Arrastrar un agente sobre la cabecera de otro pone a los dos en el mismo panel, con una fila de
pestañas arriba. Lo mismo se hace para toda un área desde el menú de la pestaña, en
[áreas de trabajo](areas-de-trabalho).

## La ventana de la app

Por voz puedes poner la ventana en un formato exacto antes de grabar: *"ventana en apaisado 1080"*,
*"ventana vertical"*, *"ventana cuadrada"*. Ver [el panel de grabación](painel-gravacao).
