---
slug: organizar-sozinho
titulo: Tidying the canvas
resumo: The command that unstacks the panels, the mode where the app arranges them for you, and named saved arrangements.
area: canvas
nivel: basico
---

## Tidy up now

Four paths do the same thing: **⌥O**, the grid button in the bottom bar, `⌘K` (type "organizar") and
voice. The key can be changed in **Settings → Shortcuts**, under "Organizar".

The command arranges the panels of the work area you are in, with no overlap, and **does not switch
the canvas mode**. 
- **The camera returns to 100%** and frames what was arranged, not the whole canvas.
- **Detached panels stay where they are.** The grid tightens to go around them. A design panel is
  never covered.
- **Images do not join the grid.** They only slide out from under the panels, into the nearest free
  spot, at the size they had.
- **The notice that appears carries the Undo**, and the same button redoes what you undid. It does
  not survive quitting the app.

## Letting the app arrange them

The two-icon switch in the bottom bar alternates between **auto grid** and **free canvas**. Switching
modes also posts a notice with Undo: going back to the grid discards the positions you set by hand.

In the **auto grid**:

- Panels fill the window and redistribute themselves when one is born, when one closes and when the
  window is resized.
- **Dragging a panel by its header swaps it** with the panel whose slot is nearest to where you
  dropped it, within the same area. Detached panels are not part of the swap.
- **The minimap in the bottom-right corner** opens the arrangements available for the number of open
  panels: **Automático**, one option per column count (from one up to the panel total) and **Foco**,
  which gives the larger space to one panel and stacks the rest. Foco uses the selected panel, or the
  first one.

In the **free canvas** nothing moves on its own. See [panels and the desk](os-paineis-e-a-mesa) and
[panning and zooming](mover-e-dar-zoom).

The mode, the chosen arrangement, the focused panel and the camera position are remembered **per work
area**.

## Saved arrangements

### Saving

A pill reading **Save recipe** appears on its own once the arrangement settles, with a name already
suggested. It only offers itself with two or more panels in the area, waits about a second without
you touching anything, disappears after a few seconds, and does not appear if the current arrangement
already matches a recipe you have.

The bookmark in the bottom bar opens the book at any time, and there you find **Save the current
one**.

### Going back

In the book, **Back** restores that row's recipe. Typing its name in `⌘K` and pressing Enter does the
same. Each row says how many panels the recipe knew, how many of them no longer exist, how many new
panels will stay on screen, and when it was made.

**Restoring never opens or closes a panel: it only positions.**

- A panel from the recipe that no longer exists is ignored.
- A panel born afterwards stays open, and is fitted into whatever space is left.
- Each panel is found again by what it is, not by an internal number: an agent by its conversation, a
  browser by its address, a file by its path, a note by which note it is.

Each row's menu has **Overwrite with the current arrangement**, **Rename** and **Delete**.

Recipes belong to each project, and store the arrangement of the work area you were in.

## By voice

- *"tidy up the windows"*, *"remove the overlap"*: the same as ⌥O.
- *"put it in two columns"*, *"three columns"*, *"focus on Perseu"*: changes the grid arrangement.
- *"save this arrangement as PR review"*: saves a recipe under that name. It touches no panel.
- *"go back to the pairing arrangement"*: restores the recipe, without opening or closing panels.
