---
slug: saber-o-que-fazem
titulo: Knowing what they're doing
resumo: Each panel's state, the back of the panel with the agent's portrait, the signals outside your view and what you can ask by voice.
area: agentes
nivel: basico
---

## The state in the panel header

The dot next to the name has five states:

- **Working**: the agent received a task or is using some tool.
- **Waiting for you**: it stopped on a question or a permission request. The dot pulses.
- **Ready**: it finished and is idle.
- **Crashed**: the answer was interrupted by an API error. See
  [creating and closing](criar-e-fechar).
- **Ended**: its process is gone.

The state stays correct with the panel minimized, in another work area or in another canvas.

## The subject line, on the panel

Below each agent's header is the subject the agent wrote about what it is doing. The whole paragraph,
and what it expects from you, appear when you hover over that line.

- **Double-clicking the line** writes a subject of your own, which the agent no longer overwrites.
  The same is in the panel's context menu, as **Write a subject…**.
- **Confirming with an empty field**, or **Return to agent** in the context menu, undoes it.
- The subject you pin does not reach the back of the panel, which keeps showing what the agent wrote.

## The back of the panel

**`⌥F`** flips every panel on the canvas at once, and `⌥F` again flips them back. The key can be
changed in **Settings → Shortcuts**, and the same thing is asked by voice with *"flip the panels"*
and *"flip them back"*.

On an agent's back:

- **The subject and the summary**, written by the agent about what it is doing.
- **What it expects from you**, when it expects something.
- **Your last task**, preceded by "you asked", once the agent has written a subject. With no subject
  written, the task appears on its own, in quotes, and an agent that has received nothing shows
  **No mission yet**.
- **What it did**: the tool count since the current task, or the step in progress while it works.
- **The state and the time**: how long it has been working, or how long the result has been sitting
  there. In the crashed state, this line shows the countdown to the next attempt, or that the app is
  waiting for the provider to come back.
- **Now** and **Delivered**, once the agent has completed something: two tabs, with the delivery
  count in the second one's label. The trail lists deliveries from the most recent to the oldest, and
  each line opens showing the summary from that moment. It can be turned off in
  [agent settings](ajustes-agentes).

## When an agent finishes out of your sight

- **Glow on the panel when done**, in **Settings → Interface**: the panel border glows when the agent
  delivers, even without being selected.
- **Highlight the area tab when done**, on the same screen: the area tab flashes when someone
  finishes or starts waiting for you in an area you are not looking at.
- **Completion glow color**, also there, applies to both, and the **Default** button undoes your
  choice.

## Asking instead of looking

With voice set up:

- ***"How is everyone doing?"***: each agent's subject.
- ***"What is Hermes doing?"***: its task, what it did and what it answered last.
- ***"Which agents do I have?"***: the ones on screen and the stored ones, with each one's subject
  and latest deliveries.
- ***"Who worked on payments?"***: searches the subject across the history of every agent in the
  project, stored ones included, and reaches the other projects if you ask.

See [what she can do](o-que-ela-consegue-fazer).

## When the agent is the one asking

The app reads the question and its options aloud and accepts a spoken answer: the option's label, its
number, or an answer of yours that isn't among the options. An answer that matches no option makes
the question be repeated instead of picked by approximation, and with two agents asking at the same
time the app asks which of them the answer is for.

Picking the option by voice works on Claude Code's multiple-choice questions. On the other CLIs the
answer goes as text, typed or dictated. See [several providers](varios-provedores).

## One agent reading another

An agent can read what another agent in this project received, did and said last, and cannot send
anything to it. See [one agent calls another](um-agente-chama-outro).

The full list, with the agents on screen and the stored ones, is in [the cast panel](painel-elenco).
