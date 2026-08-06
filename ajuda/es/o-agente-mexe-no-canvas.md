---
slug: o-agente-mexe-no-canvas
titulo: El agente trabaja el lienzo
resumo: Abrir paneles, mostrar archivos, reproducir contenido, escribir el asunto del panel y disparar anuncios.
area: agentes-fazem
nivel: basico
---

## Qué pedir

- *"Escribe el plan en un archivo y ábrelo aquí en la pantalla."*
- *"Haz el informe y muéstramelo, en vez de pegarlo todo en la terminal."*
- *"Abre el panel de Git al lado mientras trabajas."*
- *"Busca un vídeo sobre concurrencia en Swift y ponlo a rodar."*
- *"Pon una lista de concentración, solo el audio."*

## Mostrar un archivo

Un agente abre cualquier archivo del proyecto en un panel. El Markdown se renderiza y las imágenes se
muestran. La ruta es relativa a la carpeta del proyecto. Ver [el panel de archivo](painel-arquivo).

## Abrir paneles

Un agente abre los paneles del lienzo por tipo: terminal, navegador, Git, elenco, tareas, notas,
mensajes, contenido, galería, grabación, cámara, uso, rendimiento, Jira, iniciativas, diseño y los
módulos que creaste.

- **Un agente no abre otro agente.** Ese tipo no aparece en su lista, y una petición de ese tipo se
  rechaza. Los agentes los creas tú, o un agente al que mandaste llamar colegas, por otra vía
  ([el agente llama colegas](o-agente-chama-colegas)).
- No cierra ni recoloca los paneles que abriste tú.

## Reproducir contenido

Un agente pone vídeo o música en el [panel de contenido](painel-midia), que se abre si no lo estaba.
De dos formas:

- **Una dirección**: busca, elige y envía el enlace directo del vídeo, la lista o la canción.
- **Un término de búsqueda**: la lista de resultados aparece en la pantalla y la elección es tuya.

También encoge el panel en una cápsula, manteniendo el sonido, y lo devuelve a su tamaño normal.

## El asunto del panel

El agente escribe qué está haciendo: un asunto corto, un contexto de dos a cuatro frases, y qué
espera de ti, cuando espera algo.

- El asunto se convierte en la línea de contexto del panel. El contexto y el pendiente aparecen en el
  reverso del panel, y Nina los lee en voz alta cuando preguntas cómo están todos. Ver
  [saber qué están haciendo](saber-o-que-fazem).
- **El texto que fijaste a mano tiene precedencia.** Mientras exista, la línea del panel es la tuya,
  y lo que el agente anote no la sustituye.
- Cambiar de asunto cierra el anterior y lo registra como una entrega, con el contexto de aquel
  momento. Esto depende de que el historial de entregas esté activo en
  [configuración de los agentes](ajustes-agentes).
- El asunto escrito por el agente no cambia su estado (trabajando, esperando, parado, caído).

## Disparar un anuncio

Los anuncios son las alertas que escribiste en [anuncios](ajustes-anuncios), con nombre, regla,
estilo y texto. El agente dispara uno de ellos por el nombre y rellena los marcadores que faltan,
como el número de versión.

- No crea anuncios, no edita el texto y no dispara un nombre que no esté en tu lista.
- **El mismo anuncio disparado por varios agentes aparece una vez.** Si ya está en pantalla o en la
  cola, los disparos siguientes se ignoran.
- Un anuncio no interrumpe: con el micrófono abierto, con Nina en conversación o en modo reunión,
  entra en la cola y aparece cuando estés libre. Uno cada vez.
