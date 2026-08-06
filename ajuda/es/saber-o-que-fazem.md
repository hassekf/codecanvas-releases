---
slug: saber-o-que-fazem
titulo: Saber qué están haciendo
resumo: El estado de cada panel, el reverso con el retrato del agente, las señales fuera de tu vista y lo que puedes preguntar por voz.
area: agentes
nivel: basico
---

## El estado en el encabezado del panel

El punto junto al nombre tiene cinco estados:

- **Trabajando**: el agente recibió una tarea o está usando alguna herramienta.
- **Esperándote**: se detuvo en una pregunta o en una petición de permiso. El punto late.
- **Listo**: terminó y está detenido.
- **Se cayó**: la respuesta se interrumpió por un error de la API. Ver
  [crear y cerrar](criar-e-fechar).
- **Finalizado**: su proceso salió.

El estado sigue siendo correcto con el panel minimizado, en otra área de trabajo o en otro lienzo.

## La línea del asunto, en el panel

Debajo del encabezado de cada agente está el asunto que él escribió sobre lo que hace. El párrafo
entero, y lo que espera de ti, aparecen al pasar el cursor por esa línea.

- **Doble clic en la línea** escribe un asunto tuyo, que el agente ya no reescribe. Lo mismo está en
  el menú contextual del panel, en **Escribir un asunto…**.
- **Confirmar con el campo vacío**, o **Devolver al agente** en el menú contextual, lo deshace.
- El asunto que fijas no alcanza el reverso del panel, que sigue mostrando lo que el agente escribió.

## El reverso del panel

**`⌥F`** voltea todos los paneles del lienzo de una vez, y `⌥F` otra vez los devuelve. La tecla se
cambia en **Ajustes → Atajos**, y lo mismo se pide por voz con *"voltea los paneles"* y *"devuélvelos"*.

En el reverso de un agente:

- **El asunto y el resumen**, escritos por el propio agente sobre lo que está haciendo.
- **Lo que espera de ti**, cuando espera algo.
- **Tu última tarea**, precedida de "pediste", cuando el agente ya escribió un asunto. Sin asunto
  escrito, la tarea aparece sola, entre comillas, y un agente que aún no recibió nada muestra **Sin
  misión aún**.
- **Lo que hizo**: el conteo de herramientas desde la tarea actual, o el paso en curso mientras
  trabaja.
- **El estado y el tiempo**: cuánto lleva trabajando, o cuánto tiempo lleva el resultado ahí. En el
  estado de caída, esta línea muestra la cuenta atrás para el próximo intento, o que la app está
  esperando a que el proveedor vuelva.
- **Ahora** y **Entregó**, cuando el agente ya completó algo: dos pestañas, con el conteo de entregas
  en la etiqueta de la segunda. La lista muestra las entregas de la más reciente a la más antigua, y
  cada línea se abre mostrando el resumen de aquel momento. Se desactiva en
  [configuración de los agentes](ajustes-agentes).

## Cuando un agente termina fuera de tu vista

- **Brillo en el panel al terminar**, en **Ajustes → Interfaz**: el borde del panel brilla cuando el
  agente entrega, aunque no esté seleccionado.
- **Destacar la pestaña del área al terminar**, en la misma pantalla: la pestaña del área parpadea
  cuando alguien termina o pasa a esperarte en un área que no estás viendo.
- **Color del destello de conclusión**, también ahí, vale para los dos, y el botón
  **Predeterminado** deshace tu elección.

## Preguntar en vez de mirar

Con la voz configurada:

- ***"¿Cómo están todos?"***: el asunto de cada agente.
- ***"¿Qué está haciendo Hermes?"***: su tarea, lo que hizo y lo que respondió por último.
- ***"¿Qué agentes tengo?"***: los que están en pantalla y los guardados, con el asunto y las últimas
  entregas de cada uno.
- ***"¿Quién tocó los pagos?"***: busca el asunto en el historial de todos los agentes del proyecto,
  guardados incluidos, y alcanza los demás proyectos si se lo pides.

Ver [qué puede hacer ella](o-que-ela-consegue-fazer).

## Cuando el que pregunta es el agente

La app lee la pregunta y las opciones en voz alta y acepta la respuesta hablada: la etiqueta de la
opción, su número, o una respuesta tuya que no está entre las opciones. Una respuesta que no coincide
con ninguna opción hace que la pregunta se repita, en vez de elegirse por aproximación, y con dos
agentes preguntando a la vez la app pregunta para cuál de ellos es la respuesta.

Elegir la opción hablando vale para las preguntas de opción múltiple de Claude Code. En las demás
CLIs la respuesta va como texto, escrito o dictado. Ver [varios proveedores](varios-provedores).

## Un agente leyendo a otro

Un agente puede leer lo que otro agente de este proyecto recibió, hizo y dijo por último, y no puede
mandarle nada. Ver [un agente llama a otro](um-agente-chama-outro).

La lista completa, con los que están en pantalla y los guardados, está en
[el panel del elenco](painel-elenco).
