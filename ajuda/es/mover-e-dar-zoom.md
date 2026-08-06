---
slug: mover-e-dar-zoom
titulo: Mover y hacer zoom
resumo: Los gestos que mueven la cámara del lienzo, los límites del zoom, y qué cambia en pantalla cuando te alejas.
area: canvas
nivel: basico
---

## Recorrer el lienzo

- **Desplazamiento del trackpad sobre un área vacía**: mueve la cámara. Sobre un panel, el
  desplazamiento es del panel.
- **Arrastre con el botón derecho sobre un área vacía**: mueve la cámara. Sobre un panel, el botón
  derecho abre el menú de ese panel.

El cajón de archivos, el navegador de diseño, la barra de frentes y el
[estante](minimizar-e-a-estante) consumen el desplazamiento como si fueran paneles: sobre ellos, la
rueda desplaza la lista.

La cámara es de cada [área de trabajo](areas-de-trabalho). Cada pestaña guarda la posición y el zoom
en que la dejaste.

## Acercar y alejar

- **Pellizco en el trackpad**: acerca y aleja, incluso con el cursor sobre un panel.
- **⌘ con desplazamiento**: lo mismo, incluso sobre un panel.
- **Rueda del ratón sobre un área vacía**: acerca y aleja sin modificador. Sobre un panel, la rueda
  es del panel. Una imagen suelta en el lienzo no es un panel, y sobre ella la rueda sigue siendo de
  la cámara.
- **Los botones − y +**, en la esquina superior derecha: cada clic cambia el zoom en un paso fijo,
  anclado en el centro de la vista.

En los gestos, el punto bajo el cursor se queda quieto. El zoom va del 15% al 300%.

## Devolver la cámara a su sitio

- **Clic en el porcentaje**, entre el − y el +: pone el zoom al 100% y deshace el desplazamiento. La
  cuadrícula se aprieta para no tapar los paneles sueltos, y las imágenes del lienzo salen de debajo
  de lo que las escondía.
- **Clic de la rueda del ratón**: hace lo mismo. Los botones laterales del ratón no.

## Lo que deja de dibujarse a distancia

En el lienzo libre, por debajo del 40% de zoom, los navegadores, los módulos y los diseños se
convierten en un rectángulo con icono y nombre. Por encima de eso, como mucho diez de ellos siguen
dibujados a la vez, empezando por los más cercanos al centro de la vista. Los paneles de medios y de
cámara nunca entran en esa cuenta, y los agentes y terminales tampoco: esos se dibujan a cualquier
zoom. En la cuadrícula automática, todos siguen dibujados.

Nada se cierra en ese momento. El agente que estaba trabajando sigue trabajando, la página del
navegador sigue cargada, y el panel vuelve a dibujarse en cuanto te acercas.

## La cuadrícula del fondo

La cuadrícula solo se dibuja en el lienzo libre. Su espaciado es de 40 puntos y se duplica a medida
que te alejas. Los dos modos de la mesa están en [los paneles y la mesa](os-paineis-e-a-mesa).

## Encontrar un panel que salió de la vista

- **⌘⇧E**: abre el [estante](minimizar-e-a-estante), con todo lo que está abierto en este proyecto.
- **⌘K**: encuentra un panel por su nombre, en cualquier área de trabajo. Ver
  [búsqueda y comandos](busca-e-comandos).
- **⌥O**: ordena los paneles sin superposición. Ver [organizar solo](organizar-sozinho).

Por voz, *"llévame a Hermes"* lleva la cámara hasta él, cambiando antes de proyecto y de área si
está en otro sitio.

## Las teclas de los proyectos

En **Ajustes → Atajos**, en el grupo del lienzo, el bloque **Ir al proyecto 1…9**. La posición es la
de la tarjeta en la pantalla inicial, descrita en [varios canvases](varios-canvases).

El selector tiene dos modos:

- **Un modificador para las nueve posiciones**: ⌘ de fábrica, lo que da ⌘1, ⌘2, ⌘3 y así. Sin ningún
  modificador marcado, las nueve posiciones se quedan sin atajo.
- **Una tecla por posición**: cada posición recibe la combinación que grabes, y la que quede en
  blanco no tiene atajo.

El aviso de la parte superior de la pantalla de atajos lista las teclas reclamadas por dos acciones
a la vez, e incluye estas nueve.
