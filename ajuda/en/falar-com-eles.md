---
slug: falar-com-eles
titulo: Talking to the agents
resumo: Sending a task by typing, dictating or speaking, answering what they ask, spotlighting a panel and telling a crashed agent to carry on.
area: agentes
nivel: basico
---

## Typing

Click the panel and type. It is the CLI's own terminal, so its slash commands and line editing work
in there.

## Dictating

Dictation delivers the text to the **selected agent**, without going through the assistant. With no
panel selected there is no destination, and the dictation bar says so. See [dictation](ditado).

## By voice

*"Tell Hermes to run the tests"*, *"ask Atlas whether that compiled"*.

- **The text goes as you said it**, with no paraphrase.
- **A stored agent is brought back** with its whole conversation, instead of being born again.
- **Two similar names stop the delivery**: the app asks which of the two before sending anything.
- **An app verb does not become a task**: *"close Perseu"* closes his panel instead of sending the
  word into his terminal.

## Answering what they ask

In **Settings → Conversation**:

- **Answer agents by voice**: after saying aloud that an agent is waiting, the app opens the
  microphone for you to answer without touching anything. Turned off, it keeps alerting you and
  leaves the notification on screen longer, without opening the microphone.
- **Response window**: how many seconds the microphone stays open after the alert, from 0 to 15, at 6
  by default. At 0 the listening is off. The control requires voice enabled and the switch above
  turned on, and the listening happens on your Mac, with no cost per second.

What is read aloud, and how to answer by picking an option, is in
[knowing what they're doing](saber-o-que-fazem).

## Spotlighting a panel

*"Focus on Hermes"* puts his panel large on the left and rearranges the others on the right. It works
for any panel, and the ones with no name of their own are called by type: *"focus on the browser"*.
*"Unfocus"* returns everyone to the grid.

## Telling a crashed agent to carry on

*"Tell Apolo to carry on"* is a request of its own, different from typing "continue" in the terminal:
the message sent explains what happened and asks the agent to check what was left half done before
redoing anything.

- **It respects the wait between attempts**: asked during the wait, the app says in how many seconds
  it will send.
- ***"When Claude is back"*** puts the agent in the queue and only resumes when the provider leaves
  the instability.
- ***"Leave it alone"*** cancels the automatic recovery for that agent.

See [creating and closing](criar-e-fechar).

## The history of what it delivered

In **Settings → Agents**, **The agent's delivery history** comes on: each subject the agent completes
becomes a line on the back of its panel when it moves to the next subject. Turned off, the back shows
only what it is doing now.

## Commands that never end

In **Settings → Agents**, **Dev servers in their own panel** comes off. Turned on, long commands such
as a dev server or a file watcher are opened in a visible terminal panel, where you see the log and
can stop them. The classification of long commands gets it wrong sometimes.

## Telling an agent to hand off the work

With agents isolated in worktrees, the workstreams sidebar carries a hand-off button per workstream.
It merges nothing: it sends the message to the agent inside that copy of the project.

In **Settings → Interface**, in the **Workstreams sidebar** section:

- **How to hand off a finished workstream**: what the message asks for. **Infer from each
  destination** is the default and looks at how work usually lands on that branch; **Direct merge**,
  **Pull request** and **Just notify** apply to every destination in every project. The choice made
  in the sidebar's own menu overrides it, and only for that destination.
- **Edit the message**: the text sent to the agent. It has three tokens, which become the branch
  name, the destination and the verb of the chosen mode. Without the verb token, the message doesn't
  say what to do.

See [worktrees and isolation](worktrees-e-isolamento).

## Talking to an agent is not the same as an agent talking to another

An agent talks to whoever it brought onto the canvas itself, and returns the result to whoever
brought it. See [one agent calls another](um-agente-chama-outro).
