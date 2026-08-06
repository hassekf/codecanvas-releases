---
slug: painel-navegador
titulo: El panel del navegador
resumo: Los controles de la barra, qué acepta la barra de direcciones, y qué separa el navegador que es tuyo del de un agente.
area: paineis
nivel: basico
---

Una página web en un panel del lienzo, con barra de navegación propia.

## Abrir

- **`⌘K`, escribiendo "browser"**: abre un panel nuevo. Cada llamada abre uno más.
- **Por voz**: *"abre el localhost 3000"*.
- **Por un agente**, cuando quiere mostrarte una página o comprobar su propio trabajo. Mira
  [el agente ve el navegador](o-agente-ve-o-navegador).

La dirección en la que abre un navegador en blanco es una elección de cada proyecto, en
[página de inicio del navegador](ajustes-navegador). En blanco, abre en Google.

## La barra de navegación

- **Volver** y **Avanzar**: el historial de esta pestaña. Quedan no disponibles cuando no hay a
  dónde ir.
- **Recargar**: relee la página **ignorando la caché**. Es el comportamiento de una recarga forzada,
  y es siempre esa: aquí no existe una recarga común.
- **Detener**: sustituye a recargar mientras la página carga.
- **Barra de direcciones**: el primer clic selecciona la dirección entera, y el clic siguiente
  coloca el cursor.

## Qué acepta la barra de direcciones

- **Sin esquema**, `localhost`, `127.0.0.1`, `0.0.0.0` y `192.168.x.x` reciben `http://`. Todo lo
  demás recibe `https://`.
- **Con esquema**, aquí solo se cargan `http`, `https`, `file`, `about` y `data`. Una dirección con
  otro esquema se entrega a macOS, que busca una aplicación capaz de abrirla.
- **`localhost:3000` se trata como dirección**, y no como un esquema llamado `localhost`. Lo mismo
  vale para `misitio.com:8080`.

## Qué hace la página

- **La página sobrevive al cambio de lienzo**, con el mismo desplazamiento, la misma sesión iniciada
  y el mismo historial. Solo se descarta cuando el panel se cierra.
- **El zoom del lienzo es el zoom de la página**: se redibuja en la escala nueva, no se estira.
- **Una ventana nueva pedida por la página** (un `target="_blank"`, el emergente de inicio de sesión
  de un servicio) se convierte en otro panel de navegador en el lienzo. Si esa ventana se cierra
  sola tras autenticar, el panel se cierra con ella.
- **Los sitios reciben la identificación de Safari**.
- **La página que no carga dice el motivo**, con la dirección y un botón **Intentar de nuevo**.

## Tu navegador y el del agente

Las cookies están separadas por dueño: los paneles que abres **tú** comparten una sesión entre sí, y
los que abre un **agente** comparten otra. Un agente no hereda tu sesión, adonde sea que navegue y
sin importar quién se lo pidió.

## Lo que no tiene

No hay favoritos, extensiones, gestor de contraseñas ni sincronización con el navegador del sistema.
