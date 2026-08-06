---
slug: varios-provedores
titulo: Several agent CLIs
resumo: Claude Code, Codex, Grok and opencode on the same canvas: how to enable them, what works the same in all of them and what belongs to one only.
area: agentes
nivel: basico
---

In **Settings → Providers**, **Agent CLIs** has one row per CLI: Claude Code, Codex, Grok and
opencode.

- **The row's state**: **installed**, with the executable's name next to it, or **not found in
  PATH**. The app looks for each one in your shell's `PATH`.
- **The switch**: enables the CLI. A CLI that is neither installed nor enabled cannot be enabled, and
  turning off the last enabled one has no effect.
- **The install command**: appears on the row of whatever was not found, with a button that copies
  it. The app does not install or update third-party CLIs. The exception is Claude Code, which an
  agent panel offers to install in one click when it is missing.

An enabled CLI starts appearing in the three places where an agent is born: in `⌘K`, with one new
agent entry per CLI, on the command bar and in voice, which accepts the spellings transcription
produces for their names.

## What is the same in all of them

- The panel with the CLI's terminal, and its name in the header, next to the agent's name.
- Each panel's states and the alerts: working, waiting for you, ready, crashed, ended.
- The back of the panel, with the subject the agent writes about itself and the delivery history.
- Per-file authorship, before the commit. See [the Git panel](painel-git).
- Dismissing and calling back with the conversation. See [creating and closing](criar-e-fechar).
- The canvas tools: its own browser, opening panels, reading what another agent is doing and bringing
  colleagues in.

## What belongs to one CLI only

- **Picking a question's option by speaking** works on Claude Code's multiple-choice questions. On
  the others, the question is read aloud just the same and the answer goes as text, typed or
  dictated.
- **Installing and pinning the version** is Claude Code's. The **Claude Code version** menu, in
  **Settings → Agents**, pins one of the versions present on the machine and, while pinned, turns off
  automatic updating.
- **Registering installations** asks for a `.claude` folder, under **Claude installations**, on the
  same screen. An agent picks among them at creation and in the panel's context menu. See
  [accounts and profiles](contas-e-perfis).
- **opencode's model is chosen inside it**: the models it runs depend on the accounts you logged into,
  and the canvas sends it no model at all. On the others, the canvas's default model is chosen in
  [project settings](ajustes-projeto).

## Switching an agent's CLI

The panel's context menu does not switch the CLI of an existing agent: each agent lives in the CLI it
was born in, including when it is called back after being dismissed. What the menu offers is
switching its **account**, within the same CLI.
