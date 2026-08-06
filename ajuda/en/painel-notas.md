---
slug: painel-notas
titulo: The notes panel
resumo: One text block per window: switching notes, creating, renaming, deleting, and what the agents write here.
area: paineis
nivel: basico
---

Open it with `⌘K` and `nova nota`. Each panel shows one note, and the notes belong to the canvas.

The panel has no save button: the text goes to disk half a second after you stop typing, and also
when the window leaves the screen.

## The header

- **The note name**: opens the menu with every note in this canvas, most recently touched first.
  Picking one changes what this window shows.
- **New Note** (in the menu and in the button on the right): clears the writing area. The note is
  born on the first character typed; opening and closing without writing leaves nothing on disk.
- **New Notes Window**: opens another panel, so you can keep two notes in sight at once.
- **Rename…**: changes the name. Enter and clicking outside confirm, Esc cancels, and an empty name
  returns the note to its automatic title.
- **Delete**: sends the note to the trash. The window then shows the most recently touched note.
- **The name on the right side**: appears when the last hand to write there wasn't yours.

## A note's name

A note does not need a name. Unnamed, it goes by the first line of its own text, cut at 42
characters, and a note with no text at all shows up as "Nota vazia". That name is how `⌘K` finds it:
type a note's name and it opens a window on that note. See [search and commands](busca-e-comandos).

## The trash

- **Trash**, in the header menu: appears when something has been deleted, with the count next to it.
- **Restore**: returns that note to the list and shows it in the window.
- **Empty the Trash**: deletes for good what is inside it.

No voice or agent tool deletes a note.

## Who else writes here

Nina, by voice, and the agents of this canvas.

- **A note created by an agent**: opens in a panel on your screen, with its name on it.
- **A note that already exists**: the agent appends to the end, never rewrites or deletes what was
  there. It can also rename it.
- **Reading**: the agent reads the titles, or the full text of a note you mention.

See [the agent uses your lists](o-agente-usa-suas-listas).

In **Settings → Tools**, turning off the **Notas** group removes voice control and changes nothing in
the panel.

For what is left to do, instead of text to keep, use [the tasks panel](painel-tarefas).
