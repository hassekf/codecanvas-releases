---
slug: busca-e-comandos
titulo: Canvas search
resumo: ⌘K: go to an open panel, create one that doesn't exist yet, recall an agent, and open an address.
area: canvas
nivel: basico
---

Opens with **⌘K**, and the key works even with the cursor inside an agent. You can change it in
**Settings → Shortcuts**, under "Paleta de comandos".

## The result sections

Results are grouped, and the group tells you what Enter will do. The section headers are in
Portuguese in every language.

- **Ir para** (go to): moves the camera to a panel that is already open. It sees panels from every
  work area, and choosing one from another area switches areas along with it. Minimized panels are
  not listed.
- **Abrir** (open): creates a new panel from the catalog. Only agents from the CLIs enabled in
  **Settings → Providers** appear.
- **Chamar de volta** (recall): recreates an agent you dismissed in this project, with its
  conversation.
- **Ação** (action): what your phrase asks for without naming it. Tidying the panels, creating a work
  area, going back to a saved arrangement, opening an address.

With the field empty, the list shows only the **Abrir** section, ordered by what you open most often
from here.

## What else it finds

- **Work areas**, by name. Choosing one switches areas.
- **Your notes** in this project, by title. They only show up when searched for.
- **Saved arrangements**, by the name you gave them. See [tidying the canvas](organizar-sozinho).
- **Running initiative executions**, by the execution's name. Finished ones are not listed.

## The address you type

A full URL opens as it is. `github.com` becomes `https://github.com`. `localhost:3000` and
`127.0.0.1` open over `http://`. A bare number between 1024 and 65535 opens
`http://localhost:<number>`.

A file name does not become an address: `package.json` does not open in the browser.

## How a result is picked

- **Every term you type must match.** "browser media" returns neither panel, it returns nothing.
- **The verb decides between creating and going.** "new browser" creates one; "go to the browser"
  takes you to the existing one. With no verb, an open panel comes before a panel to be created.
- **Misspellings are accepted** from four letters on, and always below any exact match. "brwoser"
  finds the browser.
- **What you use most only breaks ties**, between two results with the same score.
- **The tag next to the name shows the term that matched**, when the title was not what matched.

## Keyboard

- **↑ ↓**: move through the list without taking the cursor out of the field, and wrap around at the
  end.
- **Enter**: opens the selected result.
- **Esc**: closes.

## The hint at the top of the canvas

The pill at the top of the canvas shows the key and takes no clicks. Turn it off in
**Settings → Interface**, under "Search shortcut hint"; with it off, the top holds only the area
tabs. Its text follows whatever shortcut is configured.

## Search inside Settings

The **Search settings** field, at the top of the Settings sidebar, uses the same engine. It searches
each setting's title, the explanation below it and the app's keys, and it accepts terms that are not
written on screen ("dark mode" leads to Interface, "mic" to the microphone).

The chosen result does not filter the screen: it opens the section, scrolls to the setting and
highlights it for a few seconds. **↑ ↓** move through the list, **Enter** jumps. **Esc** clears the
field, and only closes Settings when the field is already empty.

## What it does not find

It does not search inside your files or inside what the agents wrote. For that, ask an agent.
