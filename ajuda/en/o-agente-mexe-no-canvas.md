---
slug: o-agente-mexe-no-canvas
titulo: The agent works the canvas
resumo: Opening panels, showing files, playing media, writing the panel's subject and firing announcements.
area: agentes-fazem
nivel: basico
---

## What to ask for

- *"Write the plan to a file and open it here on screen."*
- *"Write the report and show it to me instead of pasting it all in the terminal."*
- *"Open the Git panel next to you while you work."*
- *"Find a video about Swift concurrency and play it."*
- *"Put on a focus playlist, audio only."*

## Showing a file

An agent opens any file in the project as a panel. Markdown is rendered and images are displayed. The
path is relative to the project folder. See [the file panel](painel-arquivo).

## Opening panels

An agent opens canvas panels by type: terminal, browser, Git, cast, tasks, notes, messages, media,
gallery, recording, webcam, usage, performance, Jira, initiatives, design and the modules you
created.

- **An agent does not open another agent.** That type is not on its list, and a request for it is
  refused. Agents are created by you, or by an agent you told to call colleagues, through another
  route ([the agent calls colleagues](o-agente-chama-colegas)).
- It does not close or reposition the panels you opened.

## Playing media

An agent puts video or music in the [media panel](painel-midia), which opens if it isn't open
already. Two ways:

- **An address**: it searches, picks one, and sends the direct link to the video, playlist or track.
- **A search term**: the list of results appears on screen and the choice is yours.

It can also shrink the panel into a capsule, keeping the sound, and bring it back to full size.

## The panel's subject

The agent writes down what it is doing: a short subject, two to four sentences of context, and what
it expects from you, when it expects something.

- The subject becomes the panel's context line. The context and the pending item appear on the back
  of the panel, and Nina reads them aloud when you ask how everyone is doing. See
  [knowing what they're doing](saber-o-que-fazem).
- **Text you pinned by hand takes precedence.** While it exists, the panel's line is yours, and
  whatever the agent writes does not replace it.
- Changing subject closes the previous one and records it as a delivery, with the context from that
  moment. This depends on the delivery history being on in [agent settings](ajustes-agentes).
- The subject written by the agent does not change its state (working, waiting, idle, crashed).

## Firing an announcement

Announcements are the alerts you wrote in [announcements](ajustes-anuncios), with a name, a rule, a
style and a text. The agent fires one of them by name and fills in the placeholders that are missing,
such as the version number.

- It does not create announcements, does not edit the text and does not fire a name that isn't on
  your list.
- **The same announcement fired by several agents appears once.** If it is already on screen or in
  the queue, further triggers are ignored.
- An announcement never interrupts: with the microphone open, with Nina in conversation or in meeting
  mode, it joins the queue and appears once you are free. One at a time.
