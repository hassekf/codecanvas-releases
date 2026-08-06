---
slug: um-agente-chama-outro
titulo: Un agente llama a otro
resumo: Delegar por voz, agentes que traen colegas al canvas, los paneles de subagente y las conversaciones entre proyectos.
area: agentes
nivel: basico
---

## Tú delegas

- **Delegar por voz**: entrega la tarea a un agente de este proyecto. Sin un agente libre, la app
  crea uno. Decir el nombre manda la tarea a ese agente, incluso a uno guardado, que vuelve solo para
  recibirla.
- **Llamar de vuelta**: trae a un agente guardado con la conversación entera. Ver
  [crear y cerrar agentes](criar-e-fechar).
- **Un nombre ambiguo no se adivina**: cuando dos nombres quedan igual de probables, la app pregunta
  cuál antes de enviar nada.

## Un agente trae colegas

Un agente en trabajo puede abrir otros agentes en el canvas, con una tarea para cada uno. Nacen con
panel, terminal y nombre propios, y cada uno puede ser de un programa de agente distinto.

- **Abrir sin tarea** deja al agente vacío, y no se le envía ningún prompt.
- **Quien los abrió recibe el resultado** de cada uno al terminar, incluso cuando la tarea sale mal.
- **Quien los abrió es despertado una vez**, cuando todos los agentes de ese pedido hayan respondido.
- **Quien los abrió puede despedir** a los agentes que trajo. El panel desaparece y la memoria queda
  guardada.
- **Nadie manda en un agente que no trajo.** Un agente puede leer lo que otro recibió, lo que ya hizo
  y lo que dijo por último, pero solo conversa con quien lo trajo o con quien él trajo.

## Los paneles de subagente

Cuando un agente divide su propio trabajo, cada división gana un panel de actividad con la tarea
recibida, las herramientas en uso y la respuesta final. El panel permanece después de concluido, y no
es una terminal.

- **Mostrar subagentes en el canvas**, en **Ajustes → Agentes**: activa y desactiva esos paneles.
  Desactivado, los subagentes trabajan igual y la app cierra los paneles que estaban abiertos.
- **El botón de subagentes de la barra de comandos**: el mismo interruptor, con el estado a la vista.
- **El tope es de tres paneles por canvas a la vez**, incluso con el interruptor activado. Un agente
  puede disparar decenas de subagentes, y los que pasen del tope trabajan sin panel.
- **Cada panel nace en el área de trabajo del agente que lo lanzó.**

## Agentes de proyectos distintos

Ninguna conversación entre proyectos empieza sola.

- **El agente pide permiso**: la pregunta aparece en tu pantalla con quién quiere hablar con quién,
  el proyecto del otro, el motivo y el saldo de mensajes. **Dejar hablar** abre la línea; **No** la
  rechaza. El mensaje que tenía guardado sale en el momento en que autorizas.
- **Tú abres una conversación por voz**, diciendo quién habla con quién y sobre qué.
- **Lo que se autoriza es la conversación**, no cada mensaje: un sí vale para ese par de agentes, ese
  tema y un saldo de mensajes contando los dos lados.
- **El saldo no se renueva con el tiempo.** Cuando se acaba, la conversación se detiene y el agente
  tiene que pedir más vueltas diciendo qué falta todavía. Ese pedido llega como una nueva pregunta en
  tu pantalla, con **Dejar continuar** y **Terminar**.
- **Conversación entre proyectos**, en **Ajustes → Agentes**: define el saldo de cada autorización.
  Las opciones son 2, 4, 6, 10 y 20 mensajes, y el valor predeterminado es 4.
- **El encabezado del panel** muestra con quién habla el agente, de qué proyecto, y cuánto del saldo
  ya se gastó. Al hacer clic en ese distintivo llegas al panel del otro agente.
- **Los asuntos de producto no cruzan**: alcance, prioridad y decidir qué construir siguen siendo
  tuyos.

## Configurado en otra pantalla

- Hablar con un agente por voz o por escrito: [hablar con los agentes](falar-com-eles).
- Qué puede hacer un agente en el canvas: [el agente llama a colegas](o-agente-chama-colegas).
- Guardar un agente y traerlo de vuelta: [minimizar y la estantería](minimizar-e-a-estante).
