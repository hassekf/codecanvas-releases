---
slug: design-no-canvas
titulo: Design on the canvas
resumo: The surface where agents draw screens and you direct by pointing, with the file versioned in the project.
area: design
nivel: basico
---

CanvasCode has a design surface of its own. **The agents draw, and you direct**: you click an element
or lasso a region and make your request from there. Each agent that is drawing shows up with a cursor
of its own on screen.

You don't edit by hand. There are no handles, no inspector and no editable text in the panel, and
your gestures on a design are two: moving artboards and pointing.

## The file

A design is a folder with a `.design` extension, which the Finder shows as if it were a file. Inside
it are the document and the images and icons it uses.

- **It usually lives in the project repository**, versioned with the code. The drawing goes into the
  history, travels to whoever clones the project, and can be read by any agent as a specification.
- **An open design is not a panel**: it opens on the canvas plane, with the artboards loose there.
- **Each screen, variation or mobile version is an artboard** inside the same file. A new file is
  born only when the subject changes.

## What you can ask for

- **Screens and variations**: *"draw three variations of the login screen: a classic one, one with a
  background photo, a minimalist one"*. A request with many screens becomes one agent per screen, all
  drawing at the same time.
- **Pointed adjustments**: select a button and ask *"make it bigger and give it more room
  underneath"*.
- **Whole flows**: *"draw the sign-up flow, four screens"*.
- **Real typography**: the agent brings a family from Google Fonts into the package, with the weights
  it uses. From then on the font travels with the file and works without internet.
- **Icons**: it uses a catalog of about two thousand icons, and whatever it uses is written into the
  package.
- **Following references**: the images you pasted on the canvas are available to it. See [images on
  the canvas](imagens-no-canvas).

What the agent does while drawing, and what it measures and checks before delivering, is in [the
agent designs and generates](o-agente-desenha-e-gera).

## The tokens

The file holds its own vocabulary of colors and measurements, and that is what every agent paints
with. Changing a token changes everything that uses it, across every artboard, at once. An agent that
needs a new color declares a token instead of writing the color loose.

## The direction

Every design has a direction written inside the file: the request, the style, the tone, the palette,
the type pairing and the rules the agent has to respect. It is what makes two agents draw the same
thing instead of two different products. See [the design direction](design-direcao).

## What it is not

- **It is not a Figma-style editor.** That is a product boundary: the ones who draw are the agents.
- **It does not export to image or to code** today.
- **It is not the image panel.** A generated image is another thing, and it lives in the
  [gallery](painel-galeria).

To write code from the drawing, an agent reads the design file itself: it is the specification, and
it needs no export.

## Where to start

1. `⌘⇧D`, or the brush in the footer, opens the design navigator.
2. **New design** asks for the direction and creates the file.
3. Choose who draws, and ask for the first screen.

The screen and the gestures are in [the design surface](painel-design).
