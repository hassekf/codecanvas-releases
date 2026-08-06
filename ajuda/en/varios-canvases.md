---
slug: varios-canvases
titulo: Several canvases
resumo: Each canvas is a project with its own folder: creating, switching without interrupting anyone, closing, and the home screen.
area: canvas
nivel: basico
---

A canvas is a project: a name and a folder. Every agent created in it is born in that folder,
described in [choosing the project](escolher-o-projeto).

## Creating

The project picker sits at the left of the command bar and shows the name of the open canvas. Click
it and choose **New canvas…**.

- **The folder is required**: the **Create** button stays unavailable until one is chosen.
- **The name is optional**: left blank, the app uses the folder's name.
- Five sections appear while creating: Project, Agents, MCP, Browser and Appearance. Skills,
  Announcements and Integrations only exist once the project has been created. See
  [project settings](ajustes-projeto).
- **By voice**, *"create a new project"* opens this same window, and the folder is chosen in it.

## Switching

- **The project picker**, in the command bar.
- **Two quick taps on ←** goes back one project, **two on →** goes forward one, wrapping around at
  the end of the list. The shortcut does not fire with any modifier held down, and does not fire
  while you are typing in an agent or in a text field.
- **⌘1 through ⌘9**, by the project's position on the home screen. The keys are changed in
  **Settings → Shortcuts**, as described in [panning and zooming](mover-e-dar-zoom).
- **By voice**: *"switch to the platform project"*.

Switching interrupts nothing. The agents of the project that left the screen keep working, and the
browsers stay as they were.

## Who is waiting in another project

The picker shows a counter when **another** canvas has agents waiting for you. Its menu breaks it
down project by project: how many are waiting, how many are working, and how many alerts arrived
there while you were away. The open project does not carry that alert count, because it is cleared
when you enter it.

## Closing a canvas

The option is at the end of the picker menu and only appears with more than one canvas. It asks for
confirmation, and what it does is this: it shuts down that project's agents and takes the canvas off
the list. The project folder and the code are untouched, and there is no undo.

Switching canvases shuts down no one. Going back to the home screen doesn't either.

## The home screen

The app opens on it, not on the last project. Each project is a card with its theme's landscape and
color, the folder path, how many agents are working there right now (or the size of the cast, if
none are) and how long ago you were in it. The last project opened gets the **WHERE YOU LEFT OFF**
mark when there is more than one.

- **RECENT PROJECTS**, below the grid: the last five you opened, in order of use. It appears from
  two projects upwards.
- **Editing a project**: the **⋯** in the card's corner, or right-clicking it.
- **Going back to the home screen** from inside a canvas: **Home screen**, at the top of the project
  picker menu.

### The order of the cards

Drag one card over another to reorder them, with the lit outline showing where it will land. The
order is saved, and it is what gives out the key: position 1 answers to ⌘1, and so on up to the
ninth. The number shows in the card's corner and next to the row in RECENT PROJECTS. From the tenth
project on there is no key.

From inside another canvas the key switches projects and the alert says the name of the one that
opened. It is the same order the two arrow taps walk through.

## What belongs to each canvas

The theme, the interface font, the background, the page a new browser opens on, the account agents
are born in, the skills, the MCP servers, the announcements, the integrations and the work areas
belong to each project. Jira connected in one does not show up in the other.

What applies to every project is under **⌘,**, the app settings. See
[project settings](ajustes-projeto) and [the look of the project](aparencia).
