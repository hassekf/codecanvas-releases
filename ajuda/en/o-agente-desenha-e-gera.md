---
slug: o-agente-desenha-e-gera
titulo: The agent designs and generates images
resumo: Asking for screens on the design surface, pointing at what to change, generating images in the canvas and using the references you pasted.
area: agentes-fazem
nivel: avancado
---

## What to ask for

- *"Design three variations of the login screen: one classic, one with a background photo, one
  minimal."*
- *"Make that button bigger and give it more room below."*
- *"Design the sign-up flow, four screens."*
- *"Bring in a better font for the headings."*
- *"Generate a fox mascot, flat, white background."*
- *"Look at the references I pasted on the canvas and follow that mood."*

What the design surface is and what it holds is in [the design panel](painel-design).

## Designing

The agent reads the design file, edits it and photographs the result. You see each change appear in
the panel as it happens.

- It creates and changes artboards, frames, rectangles, ellipses, text, paths, images and icons, with
  layout, fill, stroke, corner radius, shadow and blur.
- It defines the file's **tokens**, the vocabulary of colours and measurements every agent paints
  with.
- **A new screen, a variation or the mobile version of something goes in as an artboard in the open
  file.** A new package is only created when the subject changes or when you ask for it separately.
- **You do not draw by hand.** There are no handles, no inspector and no editable text in the panel.
  Your gestures on the design are moving screens and pointing.

## Pointing

Click an element in the design, or lasso a region, and the request gains a referent.

- The selection travels with the message: an image crop of what you pointed at, plus the identifiers
  and measurements of that fragment.
- The agent that receives the pointing is chosen in the design panel itself, and the choice is kept
  between one request and the next.
- **Seven words carry direction instructions when they appear in what you write**: `mais ousado`,
  `mais quieto`, `polir`, `mais denso`, `mais leve`, `variar` and `alinhar`. They apply to the region
  you pointed at.

## Several screens at once

A request with many screens or many variations becomes one agent per screen, each confined to its own
artboard, working at the same time. The split is done by the agent that received the request, through
the same route as [the agent calls colleagues](o-agente-chama-colegas).

## The file's direction

Every design has a written direction: the style, the product summary, the tone, the memorable thing
about the screen, the palette and the font pairing. It is filled in when the design is created, and
you can reopen and edit it later.

- An agent does not change the file's style, palette or fonts unless you ask.
- A file without a direction does not get its first element: the agent is told to write the direction
  first.

## Typography

- **Measuring**: the agent measures text with the file's real font before inserting it, and gets
  width and height in pixels. For a paragraph, it passes a maximum width and gets the height with the
  actual line breaks. The measurement covers the text alone, without the box padding.
- **Bringing in a Google Fonts family** into the package, with the weights it is going to use. The
  download runs in the background and the text switches fonts when it lands. From then on the font
  travels with the file and works offline.

## Generating images

The image is created in the canvas, in free space next to the panel of whoever asked.

- The agent chooses the count and the orientation: landscape, portrait or square.
- The model and quality come from your Settings. It can request a different quality for that call
  only, among low, medium and high.
- The model's own cap beats the requested count: some generate one image at a time.
- Every generated image goes to the [gallery](painel-galeria), with the request that created it.
- This is not the wallpaper. The screen background is changed in [appearance](aparencia).
- Generating images uses your OpenAI key, the same one as voice. Without it, the agent is told the
  key is missing.

## The references you pasted

Images you paste or drag onto the canvas become available to the agents. An agent lists those images
and opens each one by its path, and it sees what is in them.

That covers error screenshots, photos of a screen and photographed paper sketches, without you
describing in words what is in the picture.
