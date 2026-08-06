---
slug: painel-elenco
titulo: El panel del elenco
resumo: Los agentes de este proyecto en cuatro secciones, qué alcanza la búsqueda, y qué hace cada botón con un agente guardado.
area: paineis
nivel: basico
---

Los agentes de este proyecto en una lista, los que están en pantalla y los que ya fueron
descartados. Ábrelo con `⌘K` escribiendo "elenco". El panel es uno por lienzo.

La lista es del proyecto: cada lienzo tiene su elenco. Los agentes que ejecutan los pasos de una
[Iniciativa](painel-iniciativas) no entran aquí.

## Las cuatro secciones

Cada una trae su cuenta en la cabecera.

- **En pantalla**: los agentes abiertos y despiertos, con la luz de estado y lo que está haciendo
  cada uno.
- **Hibernando**: los agentes abiertos que se durmieron por inactividad. Siguen en el lienzo y
  despiertan al recibir un prompt. Quien controla esto es **Hibernar agentes inactivos**, en
  [configuración de los agentes](ajustes-agentes).
- **Guardados**: los agentes descartados que tienen una conversación por retomar, con la última
  misión entre comillas y hace cuánto estuvieron activos.
- **Guardados sin historial**: los descartados que nunca recibieron una tarea. Solo ocupan un
  nombre.

Sin ningún agente, el panel dice que el proyecto todavía no tiene ninguno; con la búsqueda escrita y
sin resultado, dice que no se encontró nada.

## La búsqueda

El campo de arriba filtra las cuatro secciones a la vez. Mira el nombre, la misión, el asunto y el
resumen que el agente anotó, su pendiente, y **todas las entregas** que registró, incluidas las de
los agentes ya descartados.

Cuando lo que coincidió con la búsqueda fue una entrega antigua, esa entrega aparece en la propia
fila, con hace cuánto fue. La misma búsqueda funciona por voz: *"¿quién trabajó en los pagos?"*.

## Los botones de cada fila

- **Ir al panel** (en la sección En pantalla): selecciona el agente y lleva la cámara hasta él.
- **Llamar** (en los guardados): reabre el agente con su conversación entera. Vuelve con el mismo
  nombre y el mismo historial.
- **Olvidar** (en los guardados, al pasar el ratón por la fila): saca al agente del elenco y libera
  el nombre. Pide confirmación, y no se puede deshacer.
- **Hacer clic en la fila** abre el resumen.

Los guardados también aparecen en el `⌘K` cuando escribes su nombre, y elegirlos ahí es lo mismo que
pulsar **Llamar**. Solo aparecen en la [búsqueda](busca-e-comandos) cuando se los busca.

## La fila abierta

- **Lo que el agente anotó**: el asunto, el resumen y el pendiente, cuando registró alguno. Sin
  resumen anotado, aparece la misión; sin ninguno de los dos, el panel dice que aún no anotó nada.
- **Entregó**: la línea de tiempo de lo que ya entregó, de la más reciente a la más antigua, con
  hace cuánto fue cada una. Muestra las seis últimas y resume el resto en una línea.

Este es el único lugar donde aparece el historial de un agente **descartado**. Para seguir a los
que están en pantalla, mira
[saber qué están haciendo](saber-o-que-fazem).

## Limpiar las secciones

- **Olvidar todos**, en la cabecera de **Guardados**: olvida a todos los que tienen conversación.
  Pide confirmación dos veces.
- **Liberar nombres**, en la cabecera de **Guardados sin historial**: los olvida a todos de una vez,
  con una sola confirmación.

En ambos casos los nombres vuelven a quedar libres para agentes nuevos, y ya no hay forma de llamar
de vuelta a quien fue olvidado.
