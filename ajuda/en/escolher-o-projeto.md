---
slug: escolher-o-projeto
titulo: Choosing the project
resumo: Creating a project, pointing at the folder, switching projects, and what happens to the agents when the folder changes.
area: comecando
nivel: basico
---

A project is a folder on your disk. **Every agent in the project is born inside it**, and that folder
is what the agents' Git, files and browser can see.

## Creating

On the start screen, **New project**. The sheet has five tabs, and only the first is required:

- **Project**: where the project lives (on this machine or on a server of yours), the folder and the
  name. With no folder chosen, the **Create** button stays unavailable.
- **Agents**: which Claude installation this project's agents are born in, and the flags passed to
  them. See [agent settings](ajustes-agentes).
- **MCP**: the servers this project's agents start. See [MCP settings](ajustes-mcp).
- **Browser**: the page a new browser opens here. See [browser settings](ajustes-navegador).
- **Appearance**: the theme, the interface font and the background. See [appearance](aparencia).

The **Skills**, **Announcements** and **Integrations** tabs only exist once the project has been
created: they depend on a real project on disk.

The project can live on another machine, with this Mac as the view. See
[remote canvas](canvas-remoto).

## Switching projects

- `⌘1` to `⌘9` open projects by their position. The key is shown in the corner of each card on the
  start screen. The modifier and the mapping can be changed in Settings → Shortcuts.
- `⌘K` finds a project by name. See [search and commands](busca-e-comandos).
- On the start screen, projects appear as cards showing the folder path, how many agents are working
  right now, and when you were last there. The one you opened last is marked.

Nothing is lost when you switch: panels stay where they were and agents keep running.

## What belongs to each project

- the canvases, the work areas and the open panels;
- the agents, on screen and stored;
- the theme, the interface font and the background. See [appearance](aparencia);
- the active skills and MCP servers;
- the announcements;
- the integrations. One project's Jira does not appear in another. See
  [integration settings](ajustes-integracoes).

One project can have several canvases. See [several canvases](varios-canvases).

## Changing the folder later

The folder is changed in [project settings](ajustes-projeto).

**An agent's folder is the folder its process was born in**, and changing the field does not reach a
terminal that is already up. With agents running, the app warns you before saving and asks:

- **Reopen with the conversation**: each agent is quit and recreated in the new folder, carrying its
  conversation along. It comes back remembering everything, and whatever it was doing at that instant
  is lost.
- **Leave in the old folder**: the processes keep running where they are, and only the next agents
  are born in the new folder.

When some agent's conversation cannot be carried over, the app names which ones before touching
anything, and you decide whether to go ahead.
