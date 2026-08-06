---
slug: design-direcao
titulo: The design direction
resumo: The brief stored inside the design file, which every agent that draws there receives before the first pixel.
area: design
nivel: basico
---

The direction is the file's brief. It is stored inside the `.design`, travels with it and applies to
**any** agent that draws there afterwards, including the ones you open tomorrow.

A file without a direction doesn't get its first element: the agent is told to write it before
drawing.

## Where it is written

- **When creating a design**: the direction screen opens before the file exists. **New design**, in
  the design navigator (`⌘⇧D`).
- **Afterwards**: the pencil on that design's row, in the navigator, reopens the screen filled in.

## What it asks for

- **Name**: the file name. Only when creating.
- **The request**: the brief, in free text. It is the only field the screen treats as necessary.
- **Direction**: one of the styles offered, or **The agent decides**.
- **Structural variance** and **Density**: two sliders, from safe to experimental and from sparse to
  dense.
- **Theme**: **Light**, **Dark** or **Both**.
- **Target**: **Desktop**, **Mobile** or **Both**.
- **Seed color**: a starting color, or **Auto**.
- **Typography**: the type pairing. Left empty, the agent chooses.
- **Who designs**: **Nobody for now**, **A new agent**, or an agent already open on the canvas.

**Whatever you leave blank, the agent chooses, declares and writes into the file.** The direction
stops having holes after the first job, and the next agent finds the decision already made instead of
inventing another one.

## The advanced rules

Four switches that come along with the direction:

- **The ban list**: the list of what may not show up in the drawing.
- **Using the file's tokens**: forces the agent to paint with the document's vocabulary of colors and
  measurements, instead of writing loose values.
- **A visual audit before delivering**: the agent takes a picture and checks its own result before
  saying it has finished.
- **A variation changes skeleton**: a variation has to change the structure, and not only the color.

## What the direction governs

- **Style, palette and fonts don't change unless you ask.** An agent that thinks it would look better
  another way proposes, it doesn't switch.
- **The pointing verbs** (*mais ousado*, *mais quieto*, *polir*, *mais denso*, *mais leve*, *variar*,
  *alinhar*) carry a direction instruction along with your request, and apply to the region you
  pointed at. See [the design surface](painel-design).
- **Each agent receives only the chapter that file calls for**, and not the whole doctrine.

## Changing the direction later

Reopening and saving applies to whatever is drawn from then on. What is already in the file stays as
it is: changing the direction repaints no artboard. To bring what already exists into line, ask.
