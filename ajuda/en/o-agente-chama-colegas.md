---
slug: o-agente-chama-colegas
titulo: The agent calls colleagues
resumo: Bringing in other agents, reading what the neighbours did, sending results back, and talking to an agent in another project.
area: agentes-fazem
nivel: basico
---

## What to ask for

- *"Bring up three agents and split the screens between them."*
- *"Call a Codex to review this, I want a second model's opinion."*
- *"Before you start, look at what Circe found out about that bug."*
- *"Who has worked on this part of the project?"*
- *"This depends on what the backend returns. Ask the people over there."*

For the side that starts with you, see [one agent calls another](um-agente-chama-outro).

## Bringing in agents

An agent creates other agents in the canvas, one panel per agent, each with its own terminal.

- **The task is optional.** With a task, the new agent is born with the request already sent. Without
  a task, it is born empty and no prompt is sent.
- Each new agent can run a different program: Claude Code, Codex, Grok or opencode. See
  [several providers](varios-provedores).
- All tasks go out in a single call. The agent that delegated ends its turn and is woken once, when
  everyone has answered, with the answers together.
- **This is not the same as internal subagents**, which don't appear on the canvas, use the same
  model and answer within the same turn. A canvas agent has its own memory, which outlives the
  conversation that created it.

## Reading colleagues

- **Read an agent**: the task it received, what it has done, and what it said last. Any agent in the
  project can read any other.
- **List the project's agents**: those on screen and those that were dismissed, with each one's last
  mission.

## Talking to colleagues

A message only reaches someone with a link: whoever the agent brought in, and whoever brought it in.

- **That is how results come back.** An agent that received a task from another answers this way when
  it finishes, including when it went wrong.
- The message carries a short summary and the paths of the files produced, not their contents.
- No agent sends a task to someone it did not bring in.

## Dismissing

An agent closes the agents it brought in itself. The panel leaves the screen and the memory is kept:
you can call the agent back from [the cast](painel-elenco) or with `⌘K`. An agent does not dismiss
someone it did not open.

## Talking to an agent in another project

**No cross-project conversation starts on its own.** The agent asks, the question appears on your
screen with the subject and the message already written, and you allow it or refuse. If refused, the
agent is told and moves on.

- What you allow is the **conversation**: a pair of agents, a subject and a message budget.
- **The default budget is 4 messages**, and the menu in Settings → Agents → "Conversations between
  projects" offers 2, 4, 6, 10 or 20. The setting is global, not per project.
- The budget does not refill over time. When it runs out, the conversation stops. The agent can ask
  for more messages, explaining exactly what is missing, and the decision is yours again.
- After asking, the agent ends its turn. It is woken when there is an answer.
- You can also open the line without waiting for the request: *"let Tristan talk to Ares on the
  backend"*.

What crosses over is system fact and agreement between the two sides: the payload format, the field
name, the unit, who validates what. Scope, priority and what the feature does do not cross over:
those questions come back to you.
