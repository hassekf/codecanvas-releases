---
slug: painel-galeria
titulo: The image gallery
resumo: This project's images kept on disk: putting one back on the canvas, deleting for real, and the prompt that generated each one.
area: paineis
nivel: basico
---

Opens with `⌘K` (type "galeria" or "imagens"). There is one per project.

## What it keeps

Every image that entered this project's canvas, whether pasted, dragged in, or generated. Removing
an image from the canvas does not delete the file: it stays here, and permanent deletion happens
**only** in this panel.

On the thumbnail and the caption:

- **Generated**: the caption is the prompt that created the image, and a badge marks it on the
  thumbnail.
- **Pasted**: the caption says only that, because there is no stored prompt.
- A second badge marks the images currently placed on the canvas.

## Grid gestures

- **Click a thumbnail**: selects and deselects. Clicking several selects several.
- **Drag starting from a gap**: draws a lasso and selects everything it touches, among the visible
  thumbnails. A click on a gap clears the selection.
- **Drag a thumbnail**: takes the image to the canvas. If it belongs to a selection of several, the
  drag takes all the selected ones, each offset from the last.
- **The `+` on hover**: puts the image back on the canvas without dragging.

## Each image's menu

- **Add to canvas**: puts the image back on the canvas.
- **Send to a contact**: sends the image through [messages](painel-recados). The prompt that
  generated it becomes the subject.
- **Copy the prompt**: copies the prompt to the clipboard. Only exists on generated images.
- **Delete from gallery**: deletes the file, with confirmation.

## The header

- **The number next to the title**: how many images the project has.
- **Delete (n)**: deletes the selected ones, with confirmation. Appears once something is selected.
- **Clear selection**: deselects everything without deleting anything.
- **Select all**, **Update** and **Clear the whole gallery**, in the menu beside them: the second
  rereads the folder from disk; the third deletes every image in the project, with confirmation.

## Deleting removes it from the canvas too

The confirmation changes when one of the images to delete is placed on the canvas: it asks **Delete
from the canvas too?** and names the work areas where the image sits. Deleting from the gallery
removes the image from the canvas as well, and there is no undo.

## How an image is generated

Ask the assistant by voice, or an agent in writing. You can say how many images you want (one is the
default), the orientation (square is the default, and there are landscape and portrait), and the
quality for that request.

Generation takes tens of seconds: the app answers before it finishes, places each image on the
canvas as it becomes ready, and reports at the end. Asked of an agent, the image appears near that
agent's panel; asked by voice, it appears in free space at the center of the view.

The prompt and the model are stored with the file. That is what the caption shows and what **Copy
the prompt** hands over.

This is not the canvas wallpaper, which has commands of its own in [appearance](aparencia).

### The default model and quality

In **Settings → Conversation**.

- **Image model**: the model that draws. The list is fetched from OpenAI, and **Update** rereads it.
- **Default image quality**: **Economy**, **Default** or **High**. It applies to requests that don't
  ask for another quality.

Both depend on your OpenAI key being set, on the same screen. See
[setting up voice](configurar-a-voz) and [what it costs](quanto-custa).

## Images loose on the canvas

Putting an image on the canvas, moving it, changing its layer and deleting it are covered in
[images on the canvas](imagens-no-canvas). This page is about where they are stored.
