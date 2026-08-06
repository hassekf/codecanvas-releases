---
slug: falar-com-eles
titulo: Hablar con los agentes
resumo: Mandar tarea escribiendo, dictando o hablando, responder lo que preguntan, destacar un panel y mandar continuar a quien se cayó.
area: agentes
nivel: basico
---

## Escribiendo

Haz clic en el panel y escribe. Es la terminal de la propia CLI, así que sus comandos de barra y la
edición de línea funcionan ahí dentro.

## Dictando

El dictado entrega el texto al **agente seleccionado**, sin pasar por la asistente. Sin ningún panel
seleccionado no hay destino, y la barra del dictado lo dice. Ver [dictado](ditado).

## Por voz

*"Dile a Hermes que corra las pruebas"*, *"pregúntale a Atlas si aquello compiló"*.

- **El texto va como lo dijiste**, sin paráfrasis.
- **Un agente guardado se trae de vuelta** con toda su conversación, en vez de nacer de nuevo.
- **Dos nombres parecidos detienen el envío**: la app pregunta cuál de los dos antes de mandar nada.
- **Un verbo de la app no se vuelve tarea**: *"cierra a Perseu"* cierra su panel en vez de mandar la
  palabra a su terminal.

## Responder lo que preguntan

En **Ajustes → Conversación**:

- **Responder a los agentes por voz**: después de avisar en voz alta que un agente espera, la app
  abre el micrófono para que respondas sin tocar nada. Desactivado, sigue avisando y deja la
  notificación más tiempo en pantalla, sin abrir el micrófono.
- **Ventana de respuesta**: cuántos segundos queda abierto el micrófono tras el aviso, de 0 a 15, en
  6 por defecto. En 0 la escucha queda desactivada. El control exige la voz activada y el interruptor
  de arriba activado, y la escucha ocurre en tu Mac, sin costo por segundo.

Lo que se lee, y cómo responder eligiendo una opción, está en
[saber qué están haciendo](saber-o-que-fazem).

## Destacar un panel

*"Foco en Hermes"* pone su panel grande a la izquierda y reorganiza los demás a la derecha. Vale para
cualquier panel, y los que no tienen nombre propio se llaman por el tipo: *"foco en el navegador"*.
*"Quita el foco"* devuelve a todos a la cuadrícula.

## Mandar continuar a quien se cayó

*"Dile a Apolo que continúe"* es una petición propia, distinta de escribir "continue" en la terminal:
el mensaje enviado cuenta qué pasó y le pide que revise lo que quedó a medias antes de rehacer nada.

- **Respeta la espera entre intentos**: pedido durante la espera, la app dice en cuántos segundos lo
  va a mandar.
- ***"Cuando Claude vuelva"*** pone al agente en la fila y solo reanuda cuando el proveedor sale de
  la inestabilidad.
- ***"Déjalo quieto"*** cancela la reanudación automática de ese agente.

Ver [crear y cerrar](criar-e-fechar).

## El historial de lo que entregó

En **Ajustes → Agentes**, **Historial de entregas del agente** viene activado: cada asunto que el
agente concluye se vuelve una línea en el reverso de su panel cuando pasa al asunto siguiente.
Desactivado, el reverso muestra solo lo que hace ahora.

## Comandos que no terminan

En **Ajustes → Agentes**, **Dev servers en su propio panel** viene desactivado. Activado, los
comandos largos como un servidor de desarrollo o un observador de archivos se abren en un panel de
terminal visible, donde ves el log y puedes interrumpirlos. La clasificación de comandos largos se
equivoca a veces.

## Mandar entregar el trabajo

Con los agentes aislados en worktrees, la barra de frentes trae un botón de entrega por frente. No
integra nada: le manda el recado al agente que está dentro de esa copia del proyecto.

En **Ajustes → Interfaz**, en la sección **Barra de frentes**:

- **Cómo entregar un frente terminado**: qué pide el recado. **Deducir de cada destino** es el valor
  por defecto y mira cómo suele entrar el trabajo en esa rama; **Merge directo**, **Pull request** y
  **Solo avisar** valen para todos los destinos de todos los proyectos. La elección hecha en el menú
  de la propia barra manda por encima, y solo en ese destino.
- **Editar el mensaje**: el texto enviado al agente. Tiene tres marcadores, que se vuelven el nombre
  de la rama, el destino y el verbo del modo elegido. Sin el marcador del verbo, el recado no dice
  qué hacer.

Ver [worktrees y aislamiento](worktrees-e-isolamento).

## Hablar con un agente no es lo mismo que un agente hablando con otro

Un agente conversa con quien él mismo trajo al lienzo, y le devuelve el resultado a quien lo trajo.
Ver [un agente llama a otro](um-agente-chama-outro).
