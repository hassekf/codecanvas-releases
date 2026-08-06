---
slug: os-paineis-e-a-mesa
titulo: Panels and the table
resumo: Opening, moving, resizing, selecting and closing panels, and the two modes the table arranges itself in.
area: canvas
nivel: basico
---

## Opening a panel

- **⌘K** and the name of what you want: terminal, browser, git, notes. See
  [search and commands](busca-e-comandos).
- **The command bar buttons**, at the bottom: **Search the canvas**, **New agent** and
  **New browser**.
- **⌘N** opens an agent, **⌘⇧N** opens a Codex agent (only with Codex enabled in
  **Settings → Providers**) and **⌘T** opens a terminal with no agent on it. All three work even
  with the cursor inside another agent.
- **By voice**: *"open a browser"*, *"open git"*.

Agents also open panels on their own. See [the agent works the canvas](o-agente-mexe-no-canvas).

## The header

Dragging by the header moves the panel. Clicking it brings the panel to the front and selects it.

- **The detach button**: takes the panel out of the automatic arrangement and gives it its own
  position and size, on top of the grid. It only exists on the automatic grid, and a detached panel
  cannot be highlighted at the same time.
- **The highlight button**: puts this panel large on the left and stacks the others in a column on
  the right. It does not appear on a detached panel. By voice, *"focus on Perseu"* and *"unfocus"*
  do the same.
- **Minimize**: puts the panel on the [shelf](minimizar-e-a-estante), with its content alive.
- **Close**: takes the panel off the canvas. A closed agent is dismissed, not deleted: see
  [creating and closing](criar-e-fechar).

Right-clicking the header opens the panel menu: writing a fixed subject for it, switching the
agent's account, minimizing, and **Move to area**, which only appears when the project has more than
one [work area](areas-de-trabalho).

## The two modes of the table

The picker is in the command bar, and the choice belongs to **each work area**: the front-end grid
does not touch the back-end one.

- **Automatic grid**: the app decides everyone's position and size. Opening or closing a panel
  redistributes the rest right away. Dragging a panel and dropping it near another swaps the two,
  within the same area.
- **Free canvas**: position and size are yours. Drag by the header to move, and pull any of the four
  sides or four corners to resize. The cursor changes as you approach the edge.

Going back to the automatic grid undoes the arrangement you built by hand. The alert shown on that
switch carries **Undo** with it.

## Choosing the grid arrangement

The minimap sits in the bottom right corner. It appears on every arrangement change and folds into
an icon after a moment, coming back when the cursor gets close. Clicking it, you choose among the
arrangements available for the number of open panels: the automatic one, from a single column up to
one column per panel, and the highlight one.

## Snapping to the grid

The **Snap to grid** button appears in the command bar **only on the free canvas**. With it on, what
you move and resize lands on 40-point steps. While dragging, only the position snaps; while
resizing, the size snaps too. It is a preference of your screen: it applies to every project.

## Selecting

- **Click**: selects a panel and brings it to the front.
- **⌘ with click**: adds to the selection, or takes out what was already marked.
- **Left-button drag over an empty area**: draws a lasso that catches everything it touches, not
  only what fits entirely inside. The selection happens during the drag.
- **Click on an empty area**: clears the selection.

Dragging a panel that is already selected takes **all** the selected ones with it.

The color, thickness and glow of the outline are in the **Selected panel** block, in the
[Appearance](ajustes-aparencia) section of the project editor. That choice applies to every canvas.

## Closing

- **The ✕ in the header** closes that panel.
- **Delete** closes the selected panels **from two upwards**. With a single panel selected, the key
  does nothing. With canvas images selected, it deletes the images instead of the panels. And it
  never fires while you are typing in a terminal or in a text field. The key is configurable in
  **Settings → Shortcuts**.
- **By voice**: *"close the agents"*, *"close two browsers"*, *"close Juno and Diana"*,
  *"close everything"*. Closing by type and *"everything"* act only on the open work area; by name,
  it reaches a panel in any area. If any target is working, the app hands the question back instead
  of closing, and it starts with the idle ones when it has to pick how many.

## Maximum width of a panel

In **Settings → Interface**, the **Maximum width of a panel** control goes from 600 to 4000 px, with
1500 px out of the box. It caps a panel that is **alone** on screen, which then sits centered;
several panels still use the whole screen. It only takes effect on the automatic grid, and it
applies to every project. By voice: *"maximum width 1500"*.

## Putting agents in a single panel

Dragging an agent onto another agent's header puts both in the same panel, with a row of tabs at the
top. The same thing is done for a whole area from the tab menu, in [work areas](areas-de-trabalho).

## The app window

By voice you can set the window to an exact shape before recording: *"window in landscape 1080"*,
*"vertical window"*, *"square window"*. See [the recording panel](painel-gravacao).
