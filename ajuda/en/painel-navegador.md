---
slug: painel-navegador
titulo: The browser panel
resumo: The toolbar controls, what the address bar accepts, and what separates the browser that is yours from an agent's.
area: paineis
nivel: basico
---

A web page in a canvas panel, with its own navigation bar.

## Opening

- **`⌘K`, typing "browser"**: opens a new panel. Every call opens one more.
- **By voice**: *"open localhost 3000"*.
- **By an agent**, when it wants to show you a page or check its own work. See
  [the agent sees the browser](o-agente-ve-o-navegador).

The address a blank browser opens at is a per-project choice, in
[browser home page](ajustes-navegador). Left empty, it opens Google.

## The navigation bar

- **Back** and **Forward**: this tab's history. They are unavailable when there is nowhere to go.
- **Reload**: reloads the page **ignoring the cache**. That is the behaviour of a forced reload, and
  it is always that one: there is no plain reload here.
- **Stop**: replaces reload while the page is loading.
- **Address bar**: the first click selects the whole address, and the next click places the cursor.

## What the address bar accepts

- **With no scheme**, `localhost`, `127.0.0.1`, `0.0.0.0` and `192.168.x.x` get `http://`.
  Everything else gets `https://`.
- **With a scheme**, only `http`, `https`, `file`, `about` and `data` are loaded here. An address
  with any other scheme is handed to macOS, which looks for an application able to open it.
- **`localhost:3000` is treated as an address**, not as a scheme called `localhost`. The same goes
  for `mysite.com:8080`.

## What the page does

- **The page survives a canvas switch**, with the same scroll position, the same login and the same
  history. It is discarded only when the panel is closed.
- **The canvas zoom is the page zoom**: the page is redrawn at the new scale rather than stretched.
- **A new window requested by the page** (a `target="_blank"`, a service's login popup) becomes
  another browser panel on the canvas. If that window closes itself after authenticating, the panel
  closes with it.
- **Sites are told the browser is Safari**.
- **A page that fails to load says why**, with the address and a **Try again** button.

## Your browser and the agent's

Cookies are separated by owner: the panels **you** open share one session among themselves, and the
ones an **agent** opens share another. An agent does not inherit your login, wherever it navigates
and whoever told it to.

## What it does not have

There are no bookmarks, extensions, password manager or syncing with the system browser.
