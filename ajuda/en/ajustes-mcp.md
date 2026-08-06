---
slug: ajustes-mcp
titulo: Settings · MCP
resumo: The screen that picks the MCP servers this project's agents spawn, installs new ones from the official registry and says what each one costs.
area: projeto
nivel: avancado
---

In **Edit the project → MCP**.

## Installed from here

The servers that came from the registry, through CanvasCode.

- **The switch** enables the server on this canvas. Every installed server is born enabled only on
  the canvas the installation came from, and dormant on the others.
- **Uninstall…**, in the row's menu: removes the server from the app's collection.

## Already configured

The servers you installed outside the app, in your agent program's account or in the project itself.
CanvasCode does not change them: here you only choose to use them on this canvas or not.

- **They all come enabled.** Turning one off stops it from being spawned for this project's next
  agents.
- **Turning them all back on** returns to inheriting the whole list, and a new server you configure
  outside the app joins on its own.
- **With no server configured outside the app**, the section says so.

## What each one costs

Each row carries a tag.

- **HTTP**: the server is shared and costs nothing per agent.
- **Process**: it spawns one process per agent, around 60 MB each. With six agents on screen, that is
  six.

CanvasCode's own MCP server, the one that gives the agent the panels, the browser and your lists,
stays out of that count: it is a single one, inside the app, shared by every agent.

## Installing

**Install…**, at the top, searches the official registry, which is public and asks for no account.

- **Each result** says whether the server speaks over HTTP or spawns a process, and whether it needs
  a key.
- **The confirmation** shows the cost, the link to the source code and the fields it needs, with the
  required ones marked. The install button stays unavailable while a required field is missing.
- **The keys go into your Mac's Keychain**, never into a file, and are handed to the server only when
  the agent is spawned.
- **Installed from a project**, the server stays enabled there and dormant on the others.

## Saving restarts the idle agents

An agent does not re-read its own arguments once it is born. When you save a change of servers, the
idle agents of this canvas are reborn with the new list, and the app tells you which ones.

- **Being reborn is not starting over**: they come back with the whole conversation and the same
  place on the canvas. What is lost is the history already painted on the terminal screen.
- **Whoever is working is not touched.** Those agents pick up the new servers the next time they are
  reborn.

## Configured elsewhere

- What an MCP server is, and what you can ask an agent: [skills and MCP servers](skills-e-mcp).
- The instructions the agents load: [Settings · Skills](ajustes-skills).
