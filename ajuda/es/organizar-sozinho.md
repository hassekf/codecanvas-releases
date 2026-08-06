---
slug: organizar-sozinho
titulo: Organizar el lienzo
resumo: El comando que desapila los paneles, el modo en que la app los ordena sola, y las disposiciones guardadas con nombre.
area: canvas
nivel: basico
---

## Organizar ahora

Cuatro caminos hacen lo mismo: **⌥O**, el botón de cuadrícula en la barra de abajo, el `⌘K` (escribe
"organizar") y la voz. La tecla se cambia en **Ajustes → Atajos**, en "Organizar".

El comando ordena los paneles del área de trabajo en la que estás, sin superposición, y **no cambia
el modo del lienzo**. 
- **La cámara vuelve al 100%** y encuadra lo que se ordenó, no el lienzo entero.
- **Los paneles sueltos se quedan donde están.** La cuadrícula se aprieta para esquivarlos. Un panel
  de diseño nunca queda cubierto.
- **Las imágenes no entran en la cuadrícula.** Solo salen de debajo de los paneles, al hueco libre
  más cercano, con el tamaño que tenían.
- **El aviso que aparece trae el Deshacer**, y el mismo botón rehace lo que deshiciste. No sobrevive
  al cierre de la app.

## Dejar que la app ordene sola

El interruptor de dos iconos de la barra de abajo alterna entre **cuadrícula automática** y **lienzo
libre**. Cambiar de modo también publica un aviso con Deshacer: volver a la cuadrícula
descarta las posiciones que montaste a mano.

En la **cuadrícula automática**:

- Los paneles llenan la ventana y se redistribuyen solos cuando nace uno, cuando se cierra otro y
  cuando la ventana cambia de tamaño.
- **Arrastrar un panel por su cabecera lo intercambia** con el panel cuyo hueco esté más cerca de
  donde lo soltaste, dentro de la misma área. Un panel suelto no entra en ese intercambio.
- **El minimapa de la esquina inferior derecha** abre las disposiciones posibles para la cantidad de
  paneles abiertos: **Automático**, una opción por número de columnas (de una hasta el total de
  paneles) y **Foco**, que da el espacio mayor a un panel y apila el resto. El Foco usa el panel
  seleccionado, o el primero.

En el **lienzo libre** nada se mueve solo. Ver [los paneles y la mesa](os-paineis-e-a-mesa) y
[mover y hacer zoom](mover-e-dar-zoom).

El modo, la disposición elegida, el panel en foco y la posición de la cámara se recuerdan **por área
de trabajo**.

## Disposiciones guardadas

### Guardar

Una píldora con **Guardar receta** aparece sola cuando la disposición se asienta, con un nombre ya
sugerido. Solo se ofrece con dos paneles o más en el área, espera cerca de un segundo sin que toques
nada, desaparece a los pocos segundos, y no aparece si la disposición actual ya es igual a una receta
que tienes.

El marcador de la barra de abajo abre el libro en cualquier momento, y allí está el **Guardar el
actual**.

### Volver

En el libro, **Volver** restaura la receta de esa fila. Escribir su nombre en el `⌘K` y pulsar Enter
hace lo mismo. Cada fila dice cuántos paneles conocía la receta, cuántos de ellos ya no existen,
cuántos paneles nuevos se quedarán en la pantalla, y de cuándo es.

**Restaurar nunca abre ni cierra un panel: solo coloca.**

- Un panel de la receta que ya no existe se ignora.
- Un panel que nació después sigue abierto, y se acomoda en el espacio que sobró.
- Cada panel se reencuentra por lo que es, y no por un número interno: un agente por su conversación,
  un navegador por su dirección, un archivo por su ruta, una nota por cuál nota es.

En el menú de cada fila están **Sobrescribir con la disposición actual**, **Renombrar** y **Borrar**.

Las recetas son de cada proyecto, y guardan la disposición del área de trabajo en la que estabas.

## Por voz

- *"organiza las ventanas"*, *"quita la superposición"*: lo mismo que el ⌥O.
- *"ponlo en dos columnas"*, *"tres columnas"*, *"foco en Perseu"*: cambia la disposición de la
  cuadrícula.
- *"guarda esta disposición como revisión de PR"*: guarda una receta con ese nombre. No toca ningún
  panel.
- *"vuelve a la disposición de pareo"*: restaura la receta, sin abrir ni cerrar paneles.
