---
slug: a-nina-por-texto
titulo: Nina por escrito
resumo: La caja de ⌘J: qué muestra, qué cerebro responde y cómo dictar dentro de ella.
area: nina
nivel: basico
---

**⌘J** abre y cierra la caja de conversación escrita, que flota sobre el lienzo. Sus ajustes están en
**Ajustes → Conversación**.

Tiene las mismas herramientas de [la conversación por voz](falar-com-a-nina) y del
[modo comando](o-modo-comando), y responde sobre el proyecto que está en tu pantalla en ese momento.
Lo que se le puede pedir está en [lo que ella puede hacer](o-que-ela-consegue-fazer).

**Las órdenes se interpretan en portugués**, igual que con la voz, así que los ejemplos de abajo están
escritos así.

## La caja

- **El campo**: escribe la petición y pulsa Enter. Vale todo lo que dirías hablando: "abre dois
  agentes do Codex", "quem está trabalhando?", "traz o Hermes de volta e manda ele rodar os testes".
- **El indicador de actividad**: mientras ella trabaja, dice el nombre de lo que se está haciendo en
  ese instante, en lugar de un progreso genérico.
- **La `×` y el clic fuera**: cierran la caja. Lo que estaba escrito en el campo sigue ahí la próxima
  vez, y una respuesta que aún venía en camino sigue llegando. Con un dictado en marcha, el clic fuera
  solo cierra la caja y no alcanza lo que está detrás.
- **Esc**: cierra la caja.

La caja nunca muestra el razonamiento ni el resultado en bruto de las herramientas.

## Qué aparece en la caja

En el menú `···`, tres modos:

- **Solo el campo**: nada más que el campo y el indicador de actividad.
- **Última respuesta**: el campo y su última frase. Es el predeterminado.
- **Conversación completa**: el hilo entero, lo que mandaste y lo que respondió.

En el mismo menú, **Ver la conversación completa** abre el historial en una ventana aparte.

## Qué cerebro responde

- **Cerebro de la conversación escrita**: elige qué CLI de agente responde cuando le escribes.
  Funciona con la suscripción que ya tienes, nunca con OpenAI. El ajuste solo aparece con más de un
  proveedor activo en Ajustes → Proveedores.

A diferencia de la conversación por voz, esta continúa donde se quedó: cerrar la app y volver más
tarde mantiene la misma conversación.

## Dictar dentro de ella

Con la caja abierta, **⌥D** dicta en el campo en lugar de mandar a un agente. La cabecera pasa a
mostrar que está escuchando, y el hilo que normalmente apunta al agente destinatario no aparece.

- **El dictado envía directo en la conversación escrita**: con esto activado, soltar la tecla ya
  envía. Apagado, el texto se queda en el campo para que lo revises y pulses Enter. Lo predeterminado
  es rellenar sin enviar. El mismo interruptor está en el menú `···` de la caja, con el nombre "Enviar
  al terminar de dictar".

Pulsar ⌥D en un lienzo sin destino para el texto, sea porque no hay agente, sea porque hay varios y
ninguno seleccionado, **abre la caja sola** antes de la primera palabra.

## La respuesta hablada

- **Leer la respuesta escrita en voz alta**: la app habla su respuesta con la voz elegida en Ajustes →
  Voz. Apagado de forma predeterminada. En [modo reunión](agenda-e-reunioes) sigue callada.

## Lo que no hace

- No abre el micrófono por su cuenta: la voz de entrada es el dictado, y la de salida es opcional.
- No lee archivos, no escribe archivos y no ejecuta comandos. El trabajo de código se lo entrega a un
  agente.
- No es la conversación con un agente. Hablar con un agente concreto sigue siendo su panel, o el
  dictado. Ver [hablar con ellos](falar-com-eles).
