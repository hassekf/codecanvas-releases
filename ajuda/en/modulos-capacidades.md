---
slug: modulos-capacidades
titulo: A module's capabilities
resumo: The bridge the app injects into the module's page: network, scripts, context, theme, storage and notifications.
area: modulos
nivel: avancado
---

The app injects a `painel` object before any script of the page. Everything returns a promise, and a
native error becomes a rejection.

- **`painel.fetch(url, opts)`**: an HTTP request made by the app, with no origin restriction. Returns
  status, body and headers.
- **`painel.executar(script, args)`**: runs an executable from its own folder, with that folder as the
  working directory; a path outside it is refused. Returns the exit code, the standard output and the
  error output, capped at 512 KB, with a 120-second limit. The process gets the workspace, the canvas
  and the module in its environment.
- **`painel.contexto()`**: the module, the canvas and the project folder this panel is in.
- **`painel.tema()`**: the accent colors and the font of the canvas theme, so the panel doesn't clash.
- **`painel.guardar(chave, valor)`** and **`painel.ler(chave)`**: a small storage, per module, shared
  across canvases. To separate it by project, include the workspace in the key.
- **`painel.notificar(opcoes)`**: an alert inside the app, with a title and a body. The options decide
  whether it is pinned or has a duration, whether it plays a sound, whether it is read aloud, and
  whether it carries a button that takes you to the panel or brings the panel to you. Repeating the
  same `id` rewrites the alert in place instead of stacking another one;
  **`painel.dispensarNotificacao(id)`** removes it from the screen. It never goes to the macOS
  Notification Center.

Keep tokens and passwords in a script in the folder, not in the HTML.

## What the page does not do

- **It doesn't navigate**: the panel shows `index.html`, and a link to the outside is ignored. Images,
  CSS and remote scripts load normally.
- **It doesn't inherit your cookies**, neither the browser panel's nor the media panel's.

## The console is captured

What the page writes to the console, JavaScript errors and rejected promises all reach the app, and
an agent reads all of it along with a picture of the panel. That's the loop for whoever is writing a
module: edit, look at the picture, read the error, fix.

There is no installing a third-party module: every module is written on your machine, by you or by
your agents.
