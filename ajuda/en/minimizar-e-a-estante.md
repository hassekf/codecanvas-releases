---
slug: minimizar-e-a-estante
titulo: Minimizing and the shelf
resumo: Putting a panel away without closing it, and the list of everything open in this project.
area: canvas
nivel: basico
---

## Minimizing

The **−** button in any panel's header, or the right-click menu → **Minimize**.

The panel leaves the screen and its content stays alive: the agent keeps working and keeps changing
state, and the browser page stays loaded, with its history and whatever you had filled in. The alert
that appears carries **Bring it back**, which restores the panel and takes the camera to it.

Two exceptions:

- **Media** becomes a pill next to the command bar, with the sound bars, play and pause. The sound
  does not stop. See [the media panel](painel-midia).
- **An agent working on a step of an Initiative** has no minimize button. In its place there is a
  hide button, which puts the panel back out of your sight without shutting anything down. See
  [the Initiatives panel](painel-iniciativas).

## Opening the shelf

- **⌘⇧E**, which also closes it.
- **The shelf button**, in the command bar. It stands out when an agent on the shelf is waiting for
  you, working, or has crashed.
- **The panel counter**, in the same bar. It shows how many panels are open on the automatic grid,
  and the camera zoom on the free canvas.

Both can be hidden in **Settings → Interface**, in the **Command bar items** block. Hidden, the item
moves behind the arrow at the end of the bar.

## What the list shows

The number at the top is the total number of panels in this canvas, across every area.

- **The area picker**, right below the title: chooses which [work area](areas-de-trabalho) the list
  belongs to. It is the same navigation as the canvas tabs: choosing here switches tabs, and
  switching tabs switches here. With a single area, it becomes a label.
- **The type filter**: **Everything**, **Agents**, **Browsers**, **Documents**, **Designs** and
  **Others**. It cuts the list inside the chosen area, and only appears when that area holds more
  than one type.
- **Each row** carries the icon, the name and, when an agent opened that panel, whose it is. An
  agent that is not idle gets a state dot next to the name.
- Panels put away drop to the end of the list and stay in their own area.

## Going to it, or bringing it to you

- **Clicking the row**: takes the camera to the panel, which stays where it is. If it was put away,
  it is restored in its own place and the camera goes along.
- **The bring button**, on the right: brings the panel to the center of your screen and, if it was
  in another area, to the open area. It only appears where the position belongs to the panel: on the
  free canvas, or on a panel detached from the grid. On the automatic grid the arrangement would
  rewrite the position an instant later.
- **The button next to it**: minimizes the panel, or takes it off the shelf and puts it back where
  it was.

## Putting away and showing in bulk

The two buttons at the bottom act on **what is listed above**: the area chosen in the picker, cut by
the filter.

- **Show**: takes every panel on the shelf in that list off it, each one in its own place. The
  camera does not move.
- **Minimize**: puts away everything that is on screen. It only appears from two upwards. The alert
  carries **Undo**, which brings back exactly those, and not everything that was put away.
