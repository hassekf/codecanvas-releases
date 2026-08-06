---
slug: painel-terminal
titulo: The terminal panel
resumo: A shell in the project folder, inside the canvas: how to open it, what the gestures do, and where the font and the name come from.
area: paineis
nivel: basico
---

A system shell running in this canvas's project folder, with no agent on top of it.

## Opening and closing

- **`⌘K`, typing "terminal"**: opens a new panel. Every call opens one more, unlike the
  [Git panel](painel-git) and the [cast panel](painel-elenco), which are one per canvas.
- **`⌘T`**: the same, without going through [search](busca-e-comandos). The key can be changed in
  Settings → Shortcuts.
- **Closing the panel ends the process.** Switching canvases does not: the shell keeps running out
  of sight, and the panel comes back with whatever it printed while you were in another project.

## The panel name

- **Double-click the title**: opens the edit field. Enter confirms, Esc cancels, and clicking away
  also confirms.
- **The terminal is the only panel with an editable name.** An agent already has a name of its own,
  and the other panels derive their title from what they show.
- **The name is an address.** It is how [search](busca-e-comandos), Nina and the agents find the
  panel: a terminal named "deploy" starts answering to "deploy" in all three.

## Gestures inside the terminal

- **Clicking a printed path**: the app looks the file up on disk and opens it wherever it reads
  best, a [file panel](painel-arquivo) for text, the browser for a web page, the Finder for
  anything else. Relative paths are resolved from the folder this terminal is in. When nothing is
  found, the app says so instead of opening an empty window.
- **Clicking a web address**: opens it in a [browser panel](painel-navegador), or in the system
  browser if this canvas is set to the external one, in the **Agents** tab of the
  [project settings](ajustes-projeto).
- **Dragging files from the Finder into it**: writes the paths, escaped, on the command line.
  Nothing is run, and no agent is involved.

## The type

- **The canvas zoom changes the font size**, not the image scale. The column count stays practically
  the same at any zoom, and the text does not rewrap as you zoom in or out.
- **Font family and starting size**: Settings → Terminal. Only monospaced fonts are offered, and the
  choice applies to every terminal and agent in the app, including the ones out of sight.

## Commands that never end

An agent running a dev server, a file watcher or any command that does not return gets stuck on it.
The app diverts those commands to a terminal panel of their own, visible on the canvas, and tells
the agent about the diversion. Commands that finish go through untouched.

That is the **Dev servers in their own panel** setting, in Settings → Agents. When off, the agent
runs everything inside itself, and a dev server ties up its conversation without showing anywhere
else. More in [talking to them](falar-com-eles).
