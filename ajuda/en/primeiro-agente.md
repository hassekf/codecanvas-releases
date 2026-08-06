---
slug: primeiro-agente
titulo: The first agent
resumo: Installing the agent program, creating the panel, sending the first task and reading the agent's state.
area: comecando
nivel: basico
---

An agent is the command-line program running inside a panel, with the whole terminal working.


## Installing the agent program

If Claude Code isn't on the machine, the new agent's panel shows **Install now**. The installation is
local and asks for no administrator password.

While the panel says **Preparing the agent…**, the app is finding out where the program lives. It
takes a few seconds.

Other agent programs run in the same canvas: Codex, Grok and opencode. Each one is enabled in
Settings → Providers. See [several providers](varios-provedores).

## Creating

- `⌘N`. It works even with the cursor inside another agent, and the new panel is born with the cursor
  in it.
- `⌘⇧N` creates a Codex agent, and the key only does something with Codex enabled in Settings.
- `⌘K`, then type **agent**.
- The new-agent button in the canvas bar.
- With voice set up, `⌥C` and *"open an agent"*.

`⌘T` opens a terminal in the same place, with no agent on top of it. See
[the terminal panel](painel-terminal).

## The name

Each agent is born with a name of its own. That is how voice, `⌘K` and the other agents address it,
and it is the name that appears in [the cast](painel-elenco) after the agent is dismissed.

## The first task

Type in the panel the way you would type in your own terminal. *"Explain what this project does"* is
a short, checkable request: it reads the files, answers, and you see the panel change state along the
way.

## The panel's state

Each panel's indicator has five states: **idle**, **working**, **waiting for you**, **crashed** and
**exited**.

**Crashed** is a turn ended by an error; **idle** is a turn completed. Automatic recovery of a
crashed agent is configured in [agent settings](ajustes-agentes).

`⌥F` flips every panel at once and shows each agent's summary: the mission, what it did and how long
ago. See [knowing what they're doing](saber-o-que-fazem).

## When it doesn't open

The panel says what is missing: the agent program not installed, or the app still locating it. For
everything else, see [when something doesn't work](quando-algo-nao-funciona).
