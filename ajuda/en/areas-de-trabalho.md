---
slug: areas-de-trabalho
titulo: Work areas
resumo: The canvas tabs: what each one holds, how to switch, and how to take panels from one to another.
area: canvas
nivel: basico
---

Work areas are the tabs at the top of the canvas. They divide a project's panels; the folder, the
Git repository and the cast of agents stay the same. To work in another folder, what you create is
another canvas: see [several canvases](varios-canvases).

Each area keeps its own panels, the mode and arrangement of the table, the camera position and zoom,
and the choice of grouping its agents into tabs or not.

## Creating and naming

- **The `+` circle**, next to the tabs: creates an area and opens its name for typing right away.
  Enter or clicking away confirms the name; Esc cancels the edit and keeps the previous one.
- **Clicking the tab you are already on**: opens its name for editing.
- **The tab's right-click menu → Rename…**: the same.
- **By voice**: *"create an area for the front end"*.

The tab bar shows even with a single area. It disappears when the workstreams sidebar is docked and
the option **Hide the area tabs while it's docked** is on, in **Settings → Interface**; there the
sidebar itself lists the areas and switches between them.

## Switching areas

- **Clicking the tab**.
- **⌃⇥ and ⌃⇧⇥**: the next one and the previous one, wrapping around at the end. With the cursor
  inside an agent, those two keys may be taken by the terminal before they reach the canvas.
- **By voice**: *"go to the back-end area"*. *"Switch to project X"* is a different thing: it
  switches canvases.

Nothing is shut down on the switch. The current area's panels leave the screen and the other area's
appear; the agent that was compiling keeps compiling.

- **The dot on a tab**: appears on tabs that are not yours, and says that someone is waiting for you
  or someone is working in that area.
- **The tab flashes** when an agent finishes or starts waiting for you in an area out of sight. That
  is turned off in **Settings → Interface**, in the **Highlight the area tab when done** control.

## Taking a panel to another area

- **Dragging the panel onto the target tab**: the tab lights up when the cursor reaches it, and a
  tag on the cursor says what is being carried. With several panels selected, all of them go, and
  the selected canvas images go along.
- **The panel's right-click menu → Move to area**: only appears with more than one area.
- **By voice**: *"send Marshall to the back-end area"*.

The agent travels alive, in the middle of whatever it is doing.

## Deleting an area

**The tab's right-click menu → Delete “name”**, available only from two areas upwards. No panel is
closed: they move to the neighboring area with their agents alive inside, and the alert says how
many went and where to.

## The agents in a single tabbed panel

**The tab's right-click menu → Group the agents into tabs**: that area's agents come to share one
panel, with a row of tabs at the top; the chosen one takes the panel and the others keep working out
of sight. **Split the agents back into panels** undoes it.

- The decision belongs to each area and overrides the app default, which is in
  **Settings → Interface**, in the **Group the agents into tabs** control.
- **Follow the app default** only appears when that area disagrees with the default, and hands the
  decision back to it.
- Dragging an agent onto another agent's header joins the two into a loose group, which coexists
  with the area's grouping.

## What crosses the areas

- **⌘K** finds panels from every area. See [search and commands](busca-e-comandos).
- **The agent list** and questions like *"who is working?"* answer for the whole project.
- **The workstreams sidebar** (**⌘⇧F**) shows the areas as sections. See
  [worktrees and isolation](worktrees-e-isolamento).
- **The shelf** shows one area at a time, chosen in the picker at its top. See
  [minimizing and the shelf](minimizar-e-a-estante).
- **Closing by type**, by voice, acts only on the open area; closing by name reaches any area. See
  [panels and the table](os-paineis-e-a-mesa).
