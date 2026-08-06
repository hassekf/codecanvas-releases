---
slug: o-que-e-um-agente
titulo: What an agent is
resumo: An agent CLI running in a real terminal inside the panel, in the canvas folder, with a name of its own.
area: agentes
nivel: basico
---

An agent is an agent CLI (Claude Code, Codex, Grok or opencode) running in a real terminal inside a
canvas panel.

## What runs in there

- **The whole program**: the slash commands, the model picker, the diffs and the permission prompts
  are the CLI's own, and you type into them as you would in Terminal.
- **The configuration already in the project**: the instructions written in the folder, the MCP
  servers and the subagents are read by the CLI, which runs in the canvas folder.
- **The binary installed on this machine**: the app looks for each CLI in your `PATH` and shows in
  **Settings → Providers** which ones it found. See [several providers](varios-provedores).

## The folder

The working directory is not chosen at creation: it comes from the canvas, and every agent created
there is born in it. See [choosing the project](escolher-o-projeto).

## The name

The name is chosen at creation, with a suggestion already filled in, and it is how you address the
agent by voice, in `⌘K` and in the cast panel.

- **While the agent exists in the project**, on screen or stored, its name is reserved and no new
  agent can take it.
- **Forgetting an agent releases the name** back to the pool of available names. See
  [creating and closing](criar-e-fechar).

## Permissions

In the canvas settings there is the **Don't ask for permission** switch, on by default. Turned off,
the CLI goes back to asking before each tool, the agent stays in the waiting state until the request
is answered, and you are notified. The permission mode menu only appears with it turned off. See
[project settings](ajustes-projeto).

## Its own browser

An agent can open a browser on the canvas, and that panel belongs to it: no other agent navigates,
clicks or takes a screenshot there. See [the agent sees the browser](o-agente-ve-o-navegador).

## The panel and the agent are different things

Closing the panel dismisses the agent and keeps the conversation, the name, the last task and what it
recorded as delivered. See [creating and closing](criar-e-fechar).
