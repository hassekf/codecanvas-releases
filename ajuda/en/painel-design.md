---
slug: painel-design
titulo: The design surface
resumo: Where the artboards live on the canvas, how to navigate them, and how pointing at something turns into a request to an agent.
area: design
nivel: avancado
---

A design file is a folder with a `.design` extension, usually kept in the project repository. It
opens **on the canvas plane**: the artboards sit loose there, with no panel frame.

- **`⌘K` and design**, **artboard**, **mockup**, **prototype**, **interface**, **layout**, **figma**,
  **wireframe** or **drawing**: opens the first `.design` in the project root. If there is none, the
  app opens the direction screen first and creates one.
- **`⌘⇧D`, or the brush in the footer**: opens the design navigator.

You don't edit by hand: there are no handles and no inspector. Your gestures on a design are moving
artboards and pointing. The agents are the ones who draw, each with a visible cursor on screen.

## The design navigator

- **On canvas**: the designs in the scene. Clicking the name collapses and expands its artboard list;
  the number next to the name counts the artboards.
- **An artboard row**: takes the camera to it. The row of the artboard in the live selection is
  highlighted.
- **The pencil**, on a design's row: reopens that file's direction, filled in.
- **The arrow**, on a design's row: takes the camera to the whole design.
- **Close design**, in the row's context menu: removes the design from the scene without deleting the
  file.
- **Remove artboard** and **Send to a contact**, in an artboard's context menu: deletes the artboard
  from the file, or sends the document to a contact, with the artboard's name as the subject.
- **In the project**: the `.design` packages in the workspace root that aren't in the scene yet.
  **Open** brings one of them to the canvas.
- **New design**: opens the direction screen and creates a file.

Pressing `⌘⇧D` again closes the navigator.

## The direction

The direction is stored inside the file and applies to any agent that draws there afterwards. The
screen asks for:

- **Name**: the file name. Only when creating.
- **The request**: the brief. It is the only field the screen treats as necessary.
- **Direction**: one of the styles offered, or **The agent decides**.
- **Structural variance** and **Density**: two sliders, from safe to experimental and from sparse to
  dense.
- **Theme** (**Light**, **Dark**, **Both**) and **Target** (**Desktop**, **Mobile**, **Both**).
- **Seed color**: a starting color, or **Auto**.
- **Typography**: the type pairing. Left empty, the agent chooses.
- **Advanced rules**: four rules the agent receives along with the rest, each with its own switch: the
  anti-slop ban list, mandatory use of the file's tokens, a visual audit before delivering, and the
  requirement that variations change skeleton.
- **Who designs**: **Nobody for now**, **A new agent**, or an agent open on the canvas. The footer
  button changes with the choice.

Whatever you leave blank the agent chooses, declares and writes into the file.

## Pointing

Click an element or lasso a region: a box appears attached to the selection.

- **The verbs** (*mais ousado*, *mais quieto*, *polir*, *mais denso*, *mais leve*, *variar*,
  *alinhar*): each tap adds the word to your text. Recognized on send, it carries a direction
  instruction to the agent.
- **The request field**: `Enter` sends.
- **The name to the right of the field**: picks the agent that receives it. The list puts agents in
  the same work area and awake ones first. The choice is remembered and isn't lost when you change
  the selection or send.

The agent receives your text, the description of what you selected, an image crop of the region, a
manifest with the ids and the file path. On a design that is still empty, the box appears all the
same and the agent is told there is no artboard yet.

The selection stays alive after sending: any agent that reads the design finds in it the referent for
*"that button"*.

## Dragging an artboard out

Pulling an artboard out of the surface turns it into a card that follows the cursor. Dropped on an
agent panel, the agent receives that artboard's citation (the crop, the ids and the file). Dropped in
empty space, nothing happens and the document doesn't change.

## The zoom

The canvas zoom and pan are the design's: there is no camera inside another camera, and the surface
doesn't scroll on its own.

## When the file has a problem

- **A file the app couldn't read**: the package is locked. The agents' tools reply with the list of
  problems and **nothing is written**. Once the file is fixed, it unlocks on its own.
- **A file changed from outside** (an agent editing `design.json` directly, a `git checkout`): the app
  reloads it. If that conflicts with what was in memory, the disk wins and the app says so.

## What the agents do here

They read the document and your selection, apply operations, take a picture of the result, measure a
text before inserting it, and bring a font from Google Fonts into the package. It's in
[the agent designs and generates](o-agente-desenha-e-gera).

Exporting the design to an image or to code doesn't exist today.
