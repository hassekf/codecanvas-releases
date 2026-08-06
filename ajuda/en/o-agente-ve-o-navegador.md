---
slug: o-agente-ve-o-navegador
titulo: The agent's browser
resumo: What an agent can do on a page open in the canvas, and how to ask it to check its own work.
area: agentes-fazem
nivel: basico
---

Each agent opens a browser of its own, as a canvas panel. The image of the page comes back to it.

## What to ask for

- *"Open localhost:3000 and tell me whether the header is aligned."*
- *"Open the page, click Sign in and tell me what happens."*
- *"The screen is blank. Read the console and tell me what the error is."*
- *"Fill the email field with an invalid value and see whether the error message shows up."*
- *"Scroll to the footer and check that the new links are there."*
- *"Tell me the text on the confirm button."*

## What it does on the page

- **Open an address**: accepts `localhost:3000`, `mysite.com:8080` or a full URL.
- **Take a picture**: returns the image of the page as it stands.
- **Click**: the target is a CSS selector (`#save`, `.btn-primary`) or the element's visible text
  (`Sign in`). The image of the result comes with it.
- **Type into a field**: the target is a CSS selector. Input events are fired, so React and Vue see
  the text. It can press Enter at the end, which covers search and login.
- **Scroll**: to the top, to the bottom, to a selector, or by a number of pixels.
- **Read the console**: logs, warnings and JavaScript errors. It is the only source when the page
  comes up blank.
- **Run JavaScript on the page**: the value of the expression comes back to it. Useful for reading an
  element's text, checking a state value or confirming that a selector exists.
- **Close the browser**: the panel leaves the canvas.

## One browser per agent

- The browser belongs to the agent that opened it. No other agent drives it.
- An agent does not drive the browser **you** opened. That one is
  [the browser panel](painel-navegador).
- If it already has a browser open, the next address goes into that same panel.

## `open` from the terminal lands in the canvas

When an agent runs `open` with a URL or with an `.html` file, CanvasCode opens the address in the
agent's browser, inside the canvas, and refuses the command. The agent gets the reason and the
address that was opened.

- This applies while this project's default browser is the internal one, in
  [browser settings](ajustes-navegador). With the external browser chosen, the command runs
  untouched.
- The escape hatch is the marker `CODECANVAS_EXTERNO=1` in front of the command: with it, the
  address opens outside the app.
- An `open .` in the Finder, an `open -a` in another program and any target that isn't a page are not
  intercepted.

## What it does not do

- It does not use Safari or Chrome to check its own work.
- It does not click an element that isn't on the page: it reports that it couldn't find it instead of
  carrying on.
