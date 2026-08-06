---
slug: iniciativas-escrever
titulo: Writing an Initiative
resumo: The two ways to create the process file by talking to an agent, and how to change it later.
area: iniciativas
nivel: avancado
---

You don't fill in any form: **the one who writes the file is an agent, talking to you**. The
Initiatives panel opens the conversation and tells the agent where to save it.

## The two ways

Both are on the panel's screen while the project still has no Initiative, and under **New initiative**
after that. In both of them you choose which agent gets it, and the conversation happens in their
panel.

### Write it from scratch, talking

The agent **doesn't read the project and doesn't propose anything** when it opens. They answer one
line saying they are ready and wait for you to tell them which process you want to describe.

From there they ask about whatever is missing, instead of filling it in on their own: the stages in
order, what each one produces, what blocks, and where somebody approves. They only save the file once
the process is settled with you.

It's the way for a process that exists in your head, or that is yet to exist.

### Read the project and propose

The agent also receives what the panel already found in the repository without reading anything: the
commands, the validation scripts and the old runs. They read those files, build the line out of what
**is written**, ask about whatever is missing instead of inventing it, save, and then tell you in five
lines what they understood, so you can check whether it matches what the team really does.

It's the way for a process that is already in the project, spread across scripts.

## What the file describes

The agent writes this; it's worth knowing what they are going to ask you:

- **How a run starts**: what the Initiative requires in order to begin, a source, a text, a list of
  questions, the output of another run, or nothing.
- **The steps, in order**: the name of each one, what goes in, what comes out, and who executes it (a
  command, or an agent with their instruction).
- **A step's gate**: the command that proves the result is good enough. With no gate, the step passes
  on the agent's word.
- **The signature**: the moment the run stops and waits for you, with what it shows and the label of
  the approve button.
- **The review**: a step whose output is a verdict, which approves, rejects or blocks the work.
- **The round ceiling** of each fixing route.

## Changing it later

On the Initiative's screen:

- **Edit with an agent**: sends the file and what you want to change to the agent you pick.
- **See the sources**: the project files the Initiative came from, each one marked as **points at**
  (the run reads today's version) or **copy** (the run uses the version saved in the Initiative).
- **See what changed**: shows up when a source file changed after the Initiative was written.
  **Re-read with the agent** sends them the file, what changed and the Initiative that came from it;
  they read it and answer what has gone stale, without touching anything.

**Editing the Initiative while a run is going changes the execution in progress**, and the run's
screen warns you when that has happened.

## When the file has an error

A file the app couldn't read shows up in the list anyway, marked, and its screen lists each refusal
with the field and the reason. The menu offers **See the problems**, **Ask an agent to fix it** and
**Open the file**.

## Where to go next

- The concept and the vocabulary: [what an Initiative is](iniciativas-o-que-e).
- Running and following: [the Initiatives panel](painel-iniciativas).
