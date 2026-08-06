---
slug: skills-e-mcp
titulo: Skills and MCP servers
resumo: What a skill and an MCP server give the agents of this project, and what you can ask an agent to do without opening a single screen.
area: agentes
nivel: avancado
---

A **skill** is an instruction file the agent loads when its subject comes up. An **MCP server** is a
program that hands tools to the agent, such as a database, an issue tracker or a company service.

Both are managed through the screens ([skills](ajustes-skills), [MCP](ajustes-mcp)) or by asking an
agent. Both paths act on the same collection.

## What an agent does with skills

- **List**: returns the skills this project has at hand, with the name, the description, the agent
  programs that see each one, and whether it is enabled on this canvas.
- **Search**: queries a public registry by subject, technology or name, and returns the candidates
  with description, stars and the source repository. Searching installs nothing. If the registry is
  down, the agent says so.
- **Install**: downloads the skill from its source repository, into the project or into your account.
  The default is the project. Asked by voice, the installation always goes into the project.
- **Write**: the agent writes the whole skill file, header included. This is what "improve this
  skill" and "merge these three into one" go through.
  A skill with the same name in the same place is overwritten, and the name becomes the folder name.
- **Enable and disable**: applies to this canvas only, and only to agents started from then on.
  Nothing leaves the disk.
- **Remove**: deletes the skill from disk, with no undo. Skills native to the agent program cannot be
  removed.

## What an agent does with MCP servers

- **List**: returns the servers CanvasCode installed, with the state of each one on this canvas, and
  the ones you configured outside the app.
- **Search**: queries the official registry, which is public and asks for no account. The result
  gives the exact name, whether the server speaks over HTTP or spawns a process, and whether it needs
  a key.
- **Install**: installs from the registry and leaves the server enabled on this canvas only. The keys
  it asks for go into the Mac's Keychain; the missing ones are left for you to fill in on the MCP
  screen.
- **Enable and disable**: applies to agents started from then on. The ones already running keep the
  servers they were born with until they are reborn.

## Where a skill lives

- **In this project**: inside the repository, versioned with the code, and therefore available to
  whoever clones the project.
- **In your account**: valid across all your projects.
- **Native to the agent program**: it ships with the program, and CanvasCode does not remove it.

When installing or writing a skill, you pick between the first two.

## Disabling is not removing

Disabling asks the agents of this project not to use that skill, and is undone with one click.
Removing deletes the file from disk with no way back. To stop using a skill here only, disable it.

## What each server costs

- **HTTP**: the server is shared and costs no process per agent.
- **Process**: it spawns one process per agent, around 60 MB each. With six agents on screen, that is
  six processes of that server.

CanvasCode's own MCP server stays out of that count: it is a single one, inside the app, shared by
every agent.

## Installing means letting third-party code run

A skill brings instructions written by someone else, and an MCP server brings code that starts
running alongside your agents. The agent confirms the source with you before installing, and a server
installed from here is born enabled only on the canvas the installation came from.

## Configured elsewhere

- The skill list of this project: [Settings · Skills](ajustes-skills).
- The MCP server list: [Settings · MCP](ajustes-mcp).
