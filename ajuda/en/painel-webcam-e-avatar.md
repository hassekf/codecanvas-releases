---
slug: painel-webcam-e-avatar
titulo: The camera and the avatar
resumo: The panel with your camera image and the panel with the assistant's face: where the controls are, when the camera turns itself off, and what changes when the panel leaves the grid.
area: paineis
nivel: basico
---

Both open with `⌘K` (type "webcam" or "avatar").

## The webcam panel

The body of the panel is the image and nothing else. The controls live in the right-click menu,
which opens both over the header and over the image:

- **Camera**: picks the image source. The list holds the cameras macOS can see right now, including
  the iPhone's Continuity Camera and Desk View. **System default** leaves the choice to macOS.
  Connecting or disconnecting a camera updates the list without reopening the panel.
- **Mirror the image**: flips the image horizontally. Capture is not restarted.

The chosen camera and mirror setting are stored in the panel, and reopening the app restores them.
If the chosen camera disappears, the panel falls back to the system default instead of going blank.

### One panel in the whole app

There is **one** webcam panel, not one per project. Opening the webcam in a canvas where it isn't
brings the panel there, and capture is not interrupted by the move.

### When the camera turns itself off

- **During a meeting**: the panel releases the camera to the call and takes it back when the meeting
  ends. See [calendar and meetings](agenda-e-reunioes).
- **With the app window closed**: the app keeps running without the window, and the camera is
  released along with it.

The camera only resumes capturing when neither reason is active.

### Out of the grid, only the image is left

With the canvas in automatic layout, the header has a **Soltar da grade** button. Out of the grid
and unselected, the webcam panel loses its header and border: only the image remains. In that state
it moves by dragging the image itself, and a click brings the controls back.

### The permission

macOS asks for camera access the first time. If access is denied, the panel shows **Camera access is
blocked** along with the path to grant it in System Settings. Authorized but with no camera
available, it shows **No camera found**. See [the permissions macOS asks for](permissoes-do-mac).

### By voice

Open the panel, mirror, unmirror, and switch cameras by saying part of the camera's name ("use the
iPhone one"). With the panel closed, the command opens it before doing the rest.

## Which camera a new panel starts with

In **Settings → Webcam**.

- **Default camera**: the camera a new webcam panel opens with.
- **Mirror the image by default**: whether a new panel starts with the image flipped.

Both apply to the **next** panel. Neither changes a panel that is already open, which keeps the
choice made in it.

## The avatar panel

The assistant's face, drawn in characters over an animated background. The drawing runs on a local
page inside the app: none of it leaves your machine.

The panel has no controls. What drives it is the voice conversation:

- when the **conversation opens**, the face condenses out of the background;
- while **she speaks**, the mouth follows the level of the voice going out;
- when the **conversation ends**, the face dissolves and the background is left.

The face takes the accent color of the theme of the canvas the panel is in, and changes along when
you switch projects. See [appearance](aparencia).

Like the webcam, the avatar is **one in the whole app**, and it loses its header and border when out
of the grid.

For what the assistant does beyond showing up, see [talking to Nina](falar-com-a-nina).
