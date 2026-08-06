---
slug: imagens-no-canvas
titulo: Images on the canvas
resumo: Pasting and dragging images onto the canvas, moving them, changing their layer and deleting them.
area: canvas
nivel: basico
---

An image pasted onto the canvas is not a panel: it doesn't take part in the automatic grid, it has no
title bar, and it stays where you left it, in either mode of the desk.

## Putting an image on the canvas

- **`⌘V`**: pastes the image from the clipboard into the middle of the view.
- **Dragging an image file** from Finder into an empty spot on the canvas: same effect.
- **Dragging a thumbnail from the gallery**, or the `+` that appears over it: puts back an image that
  is already stored. See [the gallery](painel-galeria).
- **An agent**, when generating an image you asked for: it appears in free space near that agent's
  panel. See [the agent designs and generates](o-agente-desenha-e-gera).

The file is copied into the app. The image does not point at the source folder, and it is not written
inside the project folder: deleting the original later does not remove the image from the canvas.

## Handling an image

- **Drag**: moves it. The whole image is the handle.
- **Click**: selects it and opens the image bar, with caption, opacity, **To the front**, **To the
  back** and **Delete**.
- **To the front** puts the image above the panels; **To the back** returns it to the lower layer.
- **Delete**, in that bar, removes the image from the canvas and keeps it in the gallery.
- **The Delete key**, with images selected: deletes the images instead of the selected panels.

## What it doesn't do

- **It doesn't join the automatic grid.** When the canvas is tidied up, images only move out from
  under the panels, to the nearest free spot, at the size they had. See
  [tidying up by itself](organizar-sozinho).
- **The mouse wheel over it belongs to the camera**, not to the image: it is not a panel.
- **It is not the wallpaper.** The canvas background is chosen in [appearance](aparencia).

## Taking images elsewhere

- **To another work area**: selected images travel along when you drag the selected panels onto the
  destination tab. See [work areas](areas-de-trabalho).
- **To an agent**: dropping a file **onto an agent's panel** pastes its path into that agent's prompt,
  without sending, instead of becoming an image on the canvas.
- **To another person**: from the image's menu in the gallery, under **Send to a contact**. See
  [messages](painel-recados).

## What agents see

Canvas images are available to this project's agents, which list and open each one by path and can
see their contents. That covers an error screenshot, a photo of a screen and a paper sketch, without
you describing in words what is in the picture.

## Where they are stored

Every image that lands on the canvas goes into the project's gallery, and that is where it is deleted
for good. See [the gallery](painel-galeria) and [where my data lives](onde-ficam-meus-dados).
