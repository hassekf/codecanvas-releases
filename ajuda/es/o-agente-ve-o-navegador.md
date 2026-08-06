---
slug: o-agente-ve-o-navegador
titulo: El navegador del agente
resumo: Qué hace un agente en una página abierta en el lienzo, y cómo pedirle que revise su propio trabajo.
area: agentes-fazem
nivel: basico
---

Cada agente abre un navegador propio, como panel del lienzo. La imagen de la página vuelve a él.

## Qué pedir

- *"Abre localhost:3000 y dime si el encabezado quedó alineado."*
- *"Abre la página, haz clic en Entrar y dime qué pasa."*
- *"La pantalla está en blanco. Lee la consola y dime cuál es el error."*
- *"Rellena el campo de correo con un valor inválido y mira si aparece el mensaje de error."*
- *"Desplázate hasta el pie de página y comprueba que los enlaces nuevos están."*
- *"Dime cuál es el texto del botón de confirmación."*

## Qué hace en la página

- **Abrir una dirección**: acepta `localhost:3000`, `misitio.com:8080` o una URL completa.
- **Fotografiar**: devuelve la imagen de la página tal como está.
- **Hacer clic**: el objetivo es un selector CSS (`#guardar`, `.btn-primary`) o el texto visible del
  elemento (`Entrar`). La imagen del resultado viene con él.
- **Escribir en un campo**: el objetivo es un selector CSS. Se disparan los eventos de input, así que
  React y Vue ven el texto. Puede pulsar Enter al final, lo que resuelve búsqueda e inicio de sesión.
- **Desplazar**: hasta arriba, hasta el final, hasta un selector, o un número de píxeles.
- **Leer la consola**: registros, avisos y errores de JavaScript. Es la única fuente cuando la página
  aparece en blanco.
- **Ejecutar JavaScript en la página**: el valor de la expresión vuelve a él. Sirve para leer el
  texto de un elemento, comprobar un valor de estado o verificar si existe un selector.
- **Cerrar el navegador**: el panel sale del lienzo.

## Un navegador por agente

- El navegador pertenece al agente que lo abrió. Ningún otro agente navega en él.
- Un agente no conduce el navegador que abriste **tú**. Ese es
  [el panel del navegador](painel-navegador).
- Si ya tiene un navegador abierto, la dirección siguiente va a ese mismo panel.

## El `open` de la terminal va al lienzo

Cuando un agente ejecuta `open` con una URL o con un archivo `.html`, CanvasCode abre la dirección en
el navegador de ese agente, dentro del lienzo, y rechaza el comando. El agente recibe el motivo y la
dirección que se abrió.

- Esto vale mientras el navegador predeterminado de este proyecto sea el interno, en
  [configuración del navegador](ajustes-navegador). Con el externo elegido, el comando pasa tal cual.
- La válvula de escape es el marcador `CODECANVAS_EXTERNO=1` delante del comando: con él, la
  dirección se abre fuera de la app.
- Un `open .` en el Finder, un `open -a` en otro programa y cualquier objetivo que no sea una página
  no se interceptan.

## Qué no hace

- No usa Safari ni Chrome para revisar su propio trabajo.
- No hace clic en un elemento que no existe: responde que no lo encontró, en vez de seguir adelante.
