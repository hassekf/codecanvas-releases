---
slug: areas-de-trabalho
titulo: Áreas de trabajo
resumo: Las pestañas del lienzo: qué guarda cada una, cómo cambiar, y cómo llevar paneles de una a otra.
area: canvas
nivel: basico
---

Las áreas de trabajo son las pestañas de la parte superior del lienzo. Dividen los paneles de un
proyecto; la carpeta, el Git y el elenco de agentes siguen siendo los mismos. Para trabajar en otra
carpeta, lo que se crea es otro canvas: ver [varios canvases](varios-canvases).

Cada área guarda sus paneles, el modo y la disposición de la mesa, la posición y el zoom de la
cámara, y la elección de agrupar o no sus agentes en pestañas.

## Crear y nombrar

- **El círculo `+`**, al lado de las pestañas: crea un área y abre su nombre para que escribas de
  inmediato. Enter o hacer clic fuera confirma el nombre; Esc cancela la edición y mantiene el
  anterior.
- **Hacer clic en la pestaña en la que ya estás**: abre su nombre para editarlo.
- **Menú del botón derecho de la pestaña → Renombrar…**: lo mismo.
- **Por voz**: *"crea un área para el front"*.

La barra de pestañas aparece incluso con una sola área. Desaparece cuando la barra de frentes está
anclada y la opción **Ocultar las pestañas de área cuando esté anclada** está activada, en
**Ajustes → Interfaz**; allí la propia barra de frentes lista las áreas y cambia entre ellas.

## Cambiar de área

- **Clic en la pestaña**.
- **⌃⇥ y ⌃⇧⇥**: la siguiente y la anterior, dando la vuelta al final. Con el cursor dentro de un
  agente, esas dos teclas pueden ser consumidas por la terminal antes de llegar al lienzo.
- **Por voz**: *"ve al área del back"*. *"Cambia al proyecto X"* es otra cosa: cambia de canvas.

Nada se cierra en el cambio. Los paneles del área actual salen de la pantalla y aparecen los de la
otra; el agente que estaba compilando sigue compilando.

- **El punto en una pestaña**: aparece en las pestañas que no son la tuya, y dice que alguien te
  está esperando o alguien está trabajando en esa área.
- **La pestaña parpadea** cuando un agente termina o pasa a esperarte en un área fuera de la vista.
  Eso se desactiva en **Ajustes → Interfaz**, en el control **Destacar la pestaña del área al
  terminar**.

## Llevar un panel a otra área

- **Arrastrar el panel hasta la pestaña de destino**: la pestaña se enciende cuando el cursor llega
  a ella, y una ficha en el cursor dice qué se va a llevar. Con varios paneles seleccionados van
  todos, y las imágenes seleccionadas del lienzo van con ellos.
- **Menú del botón derecho del panel → Mover al área**: solo aparece con más de un área.
- **Por voz**: *"manda a Marshall al área del back"*.

El agente viaja vivo, en medio de lo que esté haciendo.

## Borrar un área

**Menú del botón derecho de la pestaña → Borrar “nombre”**, disponible solo a partir de dos áreas.
No se cierra ningún panel: pasan al área vecina con los agentes vivos dentro, y el aviso dice
cuántos fueron y adónde.

## Los agentes en una sola pestaña

**Menú del botón derecho de la pestaña → Agrupar los agentes en pestañas**: los agentes de esa área
pasan a compartir un panel, con una fila de pestañas arriba; el elegido ocupa el panel y los demás
siguen trabajando fuera de la vista. **Separar los agentes en paneles** lo deshace.

- La decisión es de cada área y manda por encima del valor por defecto de la app, que está en
  **Ajustes → Interfaz**, en el control **Agrupar los agentes en pestañas**.
- **Seguir el valor por defecto de la app** solo aparece cuando esa área discrepa del valor por
  defecto, y le devuelve la decisión.
- Arrastrar un agente sobre la cabecera de otro junta a los dos en un grupo suelto, que convive con
  la agrupación del área.

## Lo que atraviesa las áreas

- **⌘K** encuentra paneles de todas las áreas. Ver [búsqueda y comandos](busca-e-comandos).
- **La lista de agentes** y las preguntas del tipo *"¿quién está trabajando?"* responden por todo el
  proyecto.
- **La barra de frentes** (**⌘⇧F**) muestra las áreas como secciones. Ver
  [worktrees y aislamiento](worktrees-e-isolamento).
- **El estante** muestra un área a la vez, elegida en el selector de su parte superior. Ver
  [minimizar y el estante](minimizar-e-a-estante).
- **Cerrar por tipo**, por voz, actúa solo sobre el área abierta; cerrar por nombre alcanza
  cualquier área. Ver [los paneles y la mesa](os-paineis-e-a-mesa).
