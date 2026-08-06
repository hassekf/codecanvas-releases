---
slug: painel-iniciativas
titulo: The Initiatives panel
resumo: The panel's three screens, what each button on a run does, and what happens when a run stops on you.
area: iniciativas
nivel: avancado
---

Open it with `⌘K` and **initiatives**, **runs**, **workflow**, **pipeline**, **steps** or **gate**.

An Initiative is a process written in a file under `.codecanvas/iniciativas/` in the repository. A
**run** is one execution of it.

## When there is none

The panel shows what it found in the repository with no agent involved (commands, validation scripts,
old executions) and two buttons. In both you choose the agent, and the conversation happens in the
agent's panel:

- **Write it from scratch, talking**: the agent is told the two of you are going to design a process.
- **Read the project and propose**: the agent also gets what the panel found, and proposes.

## The list

- **All**, **Running**, **Waiting on you**, **Waiting outside**, **Finished**: filter the runs. Each
  one carries its count.
- **The Initiative menu**: narrows the list to one of them. Only appears with more than one
  Initiative in the project.
- **New initiative**: picks an agent and opens the conversation to write one.
- **New run**, on an Initiative's row: starts an execution.
- **Archive**, on a finished run's row: removes the run from the list without deleting its folder.
- The button on the right of each run changes with its situation: **Reply**, **Resolve**, **Read
  what got stuck**, **Resume**, **See what's missing**, **See the result**.

An Initiative living in a [worktree](worktrees-e-isolamento) appears with the branch next to it, and
its runs happen in there.

A file the app could not read **still appears in the list**, marked, and its screen lists every
refusal with the field and the reason. Its menu offers **See the problems**, **Ask an agent to fix
it** and **Open the file**.

## One Initiative's screen

It shows the steps in order, what each one takes in and produces, who runs it (a command or an
agent), the gates, the reviews, each route's round limit, and what the Initiative needs to start.

- **New run**: starts an execution.
- **Edit with an agent**: sends the file and what you want changed to the agent you pick.
- **See the sources**: the project files the Initiative came from, each marked as **points at** (the
  run reads the current version) or **copy** (the run uses the version stored in the Initiative).
- **See what changed**: appears when a source file changed after the Initiative was written. **Re-read
  with the agent** sends it the file, what changed in it, and the Initiative that came from it.
- **Archive the finished ones** and **Delete the Initiative**, in the menu: deleting moves the
  `.json` file to the trash; the runs in the history and the project files stay where they are.

## Starting a run

**New run** asks for whatever the Initiative declared it needs: a source (a link, a card key, a
file), a text, a list of questions, another run's output, or nothing. Without that input, the start
button is unavailable.

On the same screen:

- **The run name**: suggested from what you gave, editable. The screen says whether the name already
  exists, and in that case adds a suffix.
- **Which tool**: the provider for the agents of the steps that don't pin their own.
- **On its own until it needs you**: chains the steps and only stops at the gates that ask for you, or
  if a gate gets stuck.
- **Step by step**: stops after each step and waits for you to move it along.
- **Where the code happens**: isolates the steps that write code in a worktree of their own, with the
  branch and the folder written on screen. The agent instructions come from this canvas or from
  [agent settings](ajustes-agentes), and **customize** replaces them for this run only.
- **Start the run**.

## While the run goes

- **Each step** gets its own agent, with no panel. Clicking the step opens that agent's panel;
  minimizing hides it again.
- **See the agent's panel**: the same thing, from the button.
- **Pause after this step** and **Let it run to the end**: switch the mode of a running execution.
- The app is what runs a step's gate, after the agent says it is done. If the gate fails, the work
  goes back to the agent with the reason, up to that route's round limit.
- If a step's agent dies, the app puts another one in its place up to twice. On the third, the run
  stops and says the problem was the crash.
- If the app is closed with a run going, it shows up as interrupted when you come back, and **Resume
  from here** starts it again.
- **End the run**, in the menu: interrupts whatever is happening. The artifacts already written, the
  worktree and the commits stay; an ended run does not resume.

## When the run stops on you

- **Signature**: the screen shows what the Initiative asked it to show (the document, a preview of
  what is about to happen outside the canvas, or the written request). The approval button carries
  the label the Initiative wrote. **Send back with a comment** opens the field and returns the step
  with your text; sending it back without writing anything is not possible.
- **The agent asked something**: the question came up mid-step and wasn't in the process. Answering
  approves nothing and advances no step; the text reaches the agent on its next turn.
- **Waiting outside**: the screen says what the step is waiting for. You can drop the file, paste a
  link or write what arrived, and **It arrived, go ahead** releases it. **Copy the request** copies
  what is missing, for you to send to whoever has the ball.
- **Stuck**: the round limit ran out, or the gate's command wasn't where the Initiative said. The
  buttons are **Try the gate again**, **Move on without the gate passing**, **Give it 3 more rounds**
  and **3 more, with a new agent**. When the gate's command doesn't exist, no round is spent and the
  screen says where the app looked.
- **Step by step**: at the end of each step the screen shows who would do the next one, what goes in
  and what comes out, and waits for the button.

## When it finishes

The run screen shows the artifacts, where they ended up (the folder or the branch), how many
signatures of yours it took, and how each gate passed. **Run again** starts another run of the same
Initiative. Whatever the Initiative declared it does with the result is offered as a button, never
carried out on its own.

## Knowing without the panel open

- **The pill in the command bar**: counts the project's live executions and opens the list of them,
  with each one's run and step. It counts what is alive, not what is working. By default it stays
  visible and works as a shortcut; **Hide Initiatives when nothing is pending**, in Settings →
  Interface, makes it appear only during an execution.
- **The alerts**: a run alerts you when it finishes, when it stops waiting on you, when it asks a
  question, when it gets stuck, and when what it was waiting for arrives from outside. Moving from
  one step to the next doesn't alert. Clicking the alert opens that run. With the run's panel in
  sight, the alert is not read aloud. The switches for sound, voice and macOS notification are the
  ones in [alerts and sounds](avisos-e-sons).

## Limitations

- **Editing the Initiative while a run is going changes the running execution**. The run screen
warns you when that happened.
- **An Initiative is made of that repository's commands and scripts**, and so it isn't reusable in
  another project.
