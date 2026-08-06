---
slug: iniciativas-o-que-e
titulo: What an Initiative is
resumo: Your team's working process written in a file in the repository, which CanvasCode reads, draws and conducts.
area: iniciativas
nivel: avancado
---

An **Initiative** is the process your team already follows, written in a file in the repository: the
stages in order, who does each one, what blocks, and where a person approves. CanvasCode reads that
file, draws the process and conducts the runs.

**The app doesn't implement anybody's process.** What executes is still the commands, the scripts and
the agents the project already has. The file is a lens over them, and if it and the commands
disagree, the commands win.

## The vocabulary

| Word | What it is |
|---|---|
| **Initiative** | The defined process, in a file inside the repository |
| **Run** | One execution of that process, from start to finish |
| **Step** | One stage: an agent or a command, with what goes in and what comes out |
| **Gate** | A command that proves the step's result is good enough |
| **Review** | A step whose output is a verdict, and whose effect is changing the route |

## What it is for

For work that repeats and has an order: a content line, a release flow, an investigation that always
goes through the same five stages with an approval of yours in the middle.

It isn't for a one-off task. To ask an agent for something, the way is still their panel or your
voice.

## What changes compared with sending the work yourself

- **The order doesn't get lost.** Each step receives what the previous one produced, plus a summary
  of up to three lines with what the artifact doesn't say: the risk the agent saw and the decision
  they took.
- **What says the step is done is the gate, not the agent.** The agent says they think they've
  finished; the app runs the command that proves it, and if it fails the work comes back with the
  reason.
- **Whoever reviews is always a new agent**, because reviewing your own work with the conversation
  still in your head is the weakest review there is.
- **Whoever fixes is the same agent on the first round**, and a new agent from the second on.
- **Every loop has a ceiling.** And an artifact identical to the previous round's stops right there,
  without spending the next round.
- **No agent gets called without you choosing which one.** Every button that talks to an agent opens
  the picker first and shows what is going to be sent.

## Where the files live

- **The Initiative** lives in `.codecanvas/iniciativas/` inside the repository, and is versioned with
  the code: it travels to whoever clones the project.
- **The runs** live in `.codecanvas/runs/`, outside git: they are execution, not definition.

**One Initiative belongs to one repository.** It is made of that project's commands and scripts, and
it isn't reusable in another one.

## What can happen in parallel

Inside a run, everything is a queue: one step, one agent, one input, one output. Parallelism exists
one level above, in two runs of the same Initiative at the same time, to compare results.

## Where to go next

- Writing one: [writing an Initiative](iniciativas-escrever).
- Following the runs: [the Initiatives panel](painel-iniciativas).
