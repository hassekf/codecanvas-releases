---
slug: ajustes-projeto
titulo: Project settings
resumo: The canvas window: the machine it lives on, the folder agents are born in, the name, and the other sections.
area: projeto
nivel: basico
---

Open the project picker, at the left of the command bar, and choose **Edit “project name”…**. On the
home screen, the same is reached through the **⋯** in the card's corner or by right-clicking it.

The window has a sidebar, and the first section is **Project**.

## Where this project lives

- **On this machine**: the folder is a folder on your Mac.
- **On a server of mine**: the project and its agents live on another machine, which keeps working
  with the Mac shut down. Once this is chosen, the local folder control disappears. See
  [remote canvas](canvas-remoto).

## Project folder

Every agent in this canvas is born in this folder, and it is the folder that Git, the files and the
agents' browser see. The **Choose…** button opens the macOS folder picker.

Changing the folder with agents on their feet:

- A warning appears in the section itself, before you save, saying how many agents are running in
  the old folder.
- On saving, the app asks what to do with them. **Reopen with the conversation** shuts down and
  recreates each agent in the new folder, carrying its conversation along: it comes back remembering
  everything, but whatever it was doing at that instant is lost. **Leave in the old folder** keeps
  the processes alive where they are, and only the next agents are born in the new folder.
- When some agent cannot carry its conversation, the app says which ones, by name, and how many come
  back whole, before touching anything. From there you can reopen anyway or cancel. The old
  conversation is not deleted in either case.

## Name

It is what you call the project by, in the picker, on the home screen and by voice. Left blank while
creating, the app uses the folder's name.

## Changing the project's account

If the account agents are born in changes and there are live agents that inherit it, the app asks
what to do with their conversation: **Bring the conversations over** copies each one's past into the
new account's folder, and **Start fresh on the new account** leaves that past where it is. Nothing
is deleted from the old account, and an agent that picked its own account in the panel menu is not
affected. See [accounts and profiles](contas-e-perfis).

## The other sections

- **Agents**: the Claude installation this project's agents are born in, the flags they are born
  with, whether they open pages in the internal or the external browser, and worktree isolation. See
  [accounts and profiles](contas-e-perfis) and [worktrees and isolation](worktrees-e-isolamento).
- **Skills**: the capabilities the agents here can use. See [skill settings](ajustes-skills).
- **MCP**: the tool servers the agents here start. See [MCP settings](ajustes-mcp).
- **Browser**: the page a new browser opens on. See [browser settings](ajustes-navegador).
- **Appearance**: the theme, the interface font and the background of this canvas, plus the outline
  of the selected panel, which applies to every canvas. See
  [project appearance](ajustes-aparencia).
- **Announcements**: the alerts agents fire on your screen when they meet a rule of yours. See
  [announcements](ajustes-anuncios).
- **Integrations**: this project's connections, such as Jira. See
  [integrations](ajustes-integracoes).

While **creating** a canvas, Skills, Announcements and Integrations do not appear in the sidebar:
all three need a project that already exists. They show up as soon as you save.

## The appearance preview

While this window is open, changing the theme, the wallpaper or the veil darkness changes the canvas
behind it right away. Only the **Save** button records the choice: **Cancel**, Esc and clicking
outside give back the appearance that was there before.

## This is not the same as Settings

**⌘,** opens the app settings: voice, microphone, shortcuts, interface scale, terminal font, maximum
width of a panel, notifications. All of that applies to every project. What you edit in this window
applies only to this canvas.
