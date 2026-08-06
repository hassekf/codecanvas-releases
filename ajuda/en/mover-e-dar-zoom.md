---
slug: mover-e-dar-zoom
titulo: Panning and zooming
resumo: The gestures that move the canvas camera, the zoom limits, and what changes on screen as you pull back.
area: canvas
nivel: basico
---

## Moving around the canvas

- **Trackpad scroll over an empty area**: pans the camera. Over a panel, the scroll belongs to the
  panel.
- **Right-button drag over an empty area**: pans the camera. Over a panel, the right button opens
  that panel's menu.

The file drawer, the design navigator, the workstreams sidebar and the [shelf](minimizar-e-a-estante)
take the scroll like panels do: over them, the wheel scrolls the list.

The camera belongs to each [work area](areas-de-trabalho). Every tab keeps the position and the zoom
you left it at.

## Zooming in and out

- **Pinch on the trackpad**: zooms in and out, including with the cursor over a panel.
- **⌘ with scroll**: the same, including over a panel.
- **Mouse wheel over an empty area**: zooms with no modifier. Over a panel, the wheel belongs to the
  panel. An image dropped on the canvas is not a panel, and over it the wheel still drives the
  camera.
- **The − and + buttons**, top right: each click changes the zoom by a fixed step, anchored at the
  center of the view.

In the gestures, the point under the cursor stays put. Zoom ranges from 15% to 300%.

## Putting the camera back

- **Clicking the percentage**, between − and +: sets the zoom to 100% and clears the pan. The grid
  tightens so it doesn't cover panels detached from it, and the canvas images move out from under
  whatever was hiding them.
- **Middle mouse click**: does the same. The mouse side buttons don't.

## What stops being drawn at a distance

On the free canvas, below 40% zoom, browsers, modules and designs become a rectangle with an icon
and a name. Above that, at most ten of them stay drawn at once, starting with the ones closest to
the center of the view. Media and webcam panels never count against that, and neither do agents and
terminals: those draw at any zoom. On the automatic grid, all of them stay drawn.

Nothing is shut down at that moment. The agent that was working keeps working, the browser page
stays loaded, and the panel draws again as soon as you get closer.

## The background grid

The grid is only drawn on the free canvas. Its spacing is 40 points and doubles as you pull back.
The two modes of the table are in [panels and the table](os-paineis-e-a-mesa).

## Finding a panel that went out of sight

- **⌘⇧E**: opens the [shelf](minimizar-e-a-estante), with everything open in this project.
- **⌘K**: finds a panel by name, in any work area. See [search and commands](busca-e-comandos).
- **⌥O**: tidies the panels with no overlap. See [tidying up on its own](organizar-sozinho).

By voice, *"take me to Hermes"* moves the camera to him, switching project and area first if he is
somewhere else.

## The project keys

In **Settings → Shortcuts**, in the canvas group, the **Go to project 1…9** block. The position is
the card's position on the home screen, described in [several canvases](varios-canvases).

The picker offers two modes:

- **One modifier for all nine positions**: ⌘ out of the box, which gives ⌘1, ⌘2, ⌘3 and so on. With
  no modifier selected, the nine positions have no shortcut at all.
- **One key per position**: each position gets the combination you record, and a position left blank
  has no shortcut.

The warning at the top of the shortcuts screen lists keys claimed by two actions at once, and it
includes these nine.
