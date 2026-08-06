---
slug: o-agente-chama-colegas
titulo: El agente llama colegas
resumo: Traer otros agentes, leer lo que hicieron los vecinos, devolver el resultado y hablar con un agente de otro proyecto.
area: agentes-fazem
nivel: basico
---

## Qué pedir

- *"Levanta tres agentes y reparte las pantallas entre ellos."*
- *"Llama a un Codex para revisar esto, quiero la opinión de otro modelo."*
- *"Antes de empezar, mira lo que descubrió Circe sobre ese error."*
- *"¿Quién ya trabajó en esa parte del proyecto?"*
- *"Esto depende del formato que devuelve el backend. Pregunta a la gente de allá."*

Para el lado que parte de ti, ver [un agente llama a otro](um-agente-chama-outro).

## Traer agentes

Un agente crea otros agentes en el lienzo, un panel por agente, cada uno con su terminal.

- **La tarea es opcional.** Con tarea, el agente nuevo nace con la petición ya enviada. Sin tarea,
  nace vacío y no se envía ningún prompt.
- Cada agente nuevo puede ser de otro programa: Claude Code, Codex, Grok u opencode. Ver
  [varios proveedores](varios-provedores).
- Todas las tareas salen en una sola llamada. Quien delegó termina su turno y se le despierta una
  vez, cuando todos hayan respondido, con las respuestas juntas.
- **Esto es distinto de los subagentes internos**, que no aparecen en el lienzo, usan el mismo modelo
  y responden dentro del mismo turno. Un agente del lienzo tiene memoria propia, que sobrevive a la
  conversación que lo creó.

## Leer a los colegas

- **Leer un agente**: la tarea que recibió, lo que ya hizo y lo que dijo por último. Cualquier agente
  del proyecto puede leer a cualquier otro.
- **Listar los agentes del proyecto**: los que están en pantalla y los que fueron descartados, con la
  última misión de cada uno.

## Hablar con los colegas

El mensaje solo alcanza a quien tiene vínculo: a quien el agente trajo, y a quien lo trajo a él.

- **Por ahí vuelve el resultado.** Un agente que recibió una tarea de otro responde por esa vía al
  terminar, incluso cuando salió mal.
- El mensaje lleva un resumen corto y la ruta de los archivos producidos, no su contenido.
- Ningún agente manda tarea a quien no trajo.

## Descartar

Un agente cierra los agentes que él mismo trajo. El panel sale de la pantalla y la memoria queda
guardada: puedes llamar al agente de vuelta desde [el elenco](painel-elenco) o con `⌘K`. Un agente no
descarta a quien no abrió él.

## Hablar con un agente de otro proyecto

**Ninguna conversación entre proyectos empieza sola.** El agente lo pide, la pregunta aparece en tu
pantalla con el asunto y el mensaje ya escritos, y tú autorizas o rechazas. Si rechazas, se le avisa
y sigue.

- Lo que autorizas es la **conversación**: un par de agentes, un asunto y un saldo de mensajes.
- **El saldo predeterminado es de 4 mensajes**, y el menú en Configuración → Agentes → "Conversación
  entre proyectos" ofrece 2, 4, 6, 10 o 20. El ajuste es global, no por proyecto.
- El saldo no se renueva con el tiempo. Cuando se acaba, la conversación se detiene. El agente puede
  pedir más mensajes, explicando qué falta exactamente, y la decisión vuelve a ser tuya.
- Después de pedirlo, el agente termina su turno. Se le despierta cuando haya respuesta.
- También puedes abrir la línea sin esperar la petición: *"deja que Tristán hable con Ares del
  backend"*.

Lo que atraviesa es hecho del sistema y acuerdo entre las dos partes: el formato del payload, el
nombre del campo, la unidad, quién valida qué. Alcance, prioridad y qué hace la función no
atraviesan: esas preguntas vuelven a ti.
