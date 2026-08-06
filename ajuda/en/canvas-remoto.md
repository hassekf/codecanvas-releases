---
slug: canvas-remoto
titulo: The canvas on a server
resumo: How to point a project at another machine, what the connection test checks, what happens when the network drops and what still does not work at a distance.
area: integracoes
nivel: avancado
---

A canvas can live on another machine. The agents are born and work there, and this Mac is the view.
The app reaches the server over SSH, and installs nothing and leaves nothing listening on the other
side.

This part of CanvasCode is under construction. What does not work yet is at the end of the page.

## Choosing the machine

In **Edit the project → Project → Where this project lives**.

- **On this machine** and **On a server of mine**: decide where this canvas's agents work. Picking
  the server hides the local folder field.
- **The server menu** lists the registered ones and brings **Add server…**. A registered server
  belongs to the app, not to the canvas: the same machine serves several projects.
- **Switching servers clears the chosen folder**.
- **Edit…**: reopens that server's registration.

## Registering a server

- **Nickname**: how that server appears in the list and how the voice refers to it.
- **Address**: the IP or the domain, the user and the SSH port.
- **Key**: the path of the private key. Left blank, the app uses the key you already use to get into
  that machine.
- **Test connection**: says whether it reached the machine, which system it is, and whether git,
  tmux, node and the agent program are there. When the agent program is installed but has no
  credential, the test warns you: without it the agent starts up, stays silent and looks stuck.
- **Save** is unavailable while the address is empty.

## Choosing the folder

**Choose folder…** opens a browser through the server's folders.

- **Up** goes one level up, and **New folder…** creates a folder there.
- **Folders that are a repository** come marked.
- **Use this folder** closes the browser with your choice. The app prepares the rest on its own.

## What works the same

- **Each agent's terminal**, with its whole screen.
- **The agent's state**: the panel light, the subject, who wrote in each file, the pending question.
- **The Git of the repository over there**, in the usual panel.
- **The file drawer**, and opening a file in a panel to read.
- **Dragging a file onto an agent**: the file is uploaded to the server first, and the agent receives
  the path over there. If the upload fails, nothing is pasted into the prompt and the app says why.

## When the network drops

The SSH of an agent that dies is not the agent dying: the session stays alive on the other side.

- **The warning appears on the panel's own screen**, saying which connection dropped and in how many
  seconds the app tries again.
- **The wait grows with each attempt**, from 3 seconds up to a ceiling of 30.
- **On reconnecting, the session is found again** with the history and the pending question where
  they were.
- **A closed panel does not reconnect.** The agent stays alive on the server, and you bring it back
  like any stored agent.

## If you log in as root

The agent program refuses to run as root with permissions waived. In that case the app drops that
option: the agent starts up and goes back to asking permission before each tool, and the app handles
those requests as always. The connection test warns you when the user is root.

## What still does not work

- **Editing a remote file**: the panel opens and shows the content, and the edit button does not
  appear.
- **Following a remote file live**: it is not watched like a local one, and is re-read when you ask.
- **The agent's browser is a panel on this Mac.** Without the Mac running, the remote agent cannot
  see the page it produced.
- **Modules are served by the app**, and therefore only exist with the Mac running.
- **The Usage and Performance panels** measure this machine.
- **Two Macs on the same canvas** do not combine yet.

## Configured elsewhere

- The folder of a local project: [project settings](ajustes-projeto).
- Switching projects: [choosing the project](escolher-o-projeto).
