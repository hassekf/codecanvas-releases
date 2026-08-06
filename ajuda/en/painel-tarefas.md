---
slug: painel-tarefas
titulo: The tasks panel
resumo: The project list: taking note, changing state, setting deadlines, the history of each line and the deadline alert.
area: paineis
nivel: basico
---

Open it with `⌘K` and `tarefas`. There is one panel per canvas, and the list belongs to the canvas:
two canvases have two lists, even when they point at the same folder.

## Taking note

- **The field at the top**: creates a task with the text you typed. Enter and the **Take note**
  button do the same thing. The deadline is not asked for here.

## The list

Three sections, in this order: **Fazendo** (doing), **Abertas** (open) and **Feitas** (done).

- **Fazendo** and **Abertas**: sorted by the nearest deadline. Tasks with no deadline go to the end.
- **Feitas**: collapsed, with the count next to the title. It opens when clicked, and also on its own
  when you complete a task. Inside it, the most recent comes first.
- **The footer**: counts how many tasks are pending and how many are overdue.

Each line shows the task text, its number, the state in words, the deadline, who touched it last and
how many comments it has.

- **The number (`#3`)**: identifies the task for voice and for the agents. It is unique within the
  canvas and never reused, and reordering the list renumbers nothing.
- **The name of who touched it last**: shown only when it wasn't you.
- **The last comment**: stays visible on the line when it was written by an agent or by Nina.
- **The bar on the left edge**: marks a task whose deadline has passed. A completed task never gets
  the bar, even with the deadline gone.

## Changing the state

- **The circle on the left**: marks the task as done, and reopens one that is already done. It does
  not pass through "in progress".
- **Start** and **Pause**: appear on the line under the cursor. **Start** moves an open task to in
  progress; **Pause** sends one in progress back to open.
- **The state written on the line**: it is a menu, and moves the task to any of the three states.
- **The line's context menu**: repeats the three states, the deadline and **Delete**.

## The deadline

The deadline is optional. From the line's context menu, under **Deadline**:

- **Today**, **Tomorrow** and **Next week**: set that day at 6 pm, and the line shows the day only.
- **Remove the due date**: appears only when a deadline exists.

A deadline with a time is set by voice ("deliver Friday at 5 pm") or by an agent. With no time, the
deadline falls at 6 pm. An overdue deadline is written as "venceu às 13h" or "venceu 4 de agosto".

## The back of a line

Clicking the line opens its back, and clicking again closes it.

- **The comments**: all of them, with the author and when they were written.
- **Comment…**: adds a comment of your own.
- **History**: every creation, state change, rewrite, deadline, comment, deletion and restore, with
  the name of who did it and when. The name stays recorded there even after the agent is dismissed.

## The trash

- **Delete**: sends the task to the trash, and the history records who deleted it. An agent deletes
  through the same door.
- **Trash**, in the footer: shows what was deleted, with **Restore** on each line.
- **Empty**: deletes for good what is in the trash. No voice or agent tool reaches this button.

## The deadline alert

A task with a deadline alerts you three times: 1 hour before, 30 minutes before and at the deadline.
Each mark alerts once only, and reopening the app does not repeat what was already said. When more
than one mark comes at once, only the most urgent one is spoken.

- **The alert covers every canvas**, not only the one in front of you. When the task belongs to
  another project, the alert says which.
- **Clicking the alert**: switches to that task's canvas and opens the tasks panel.
- Turning it on and off, muting it and having it read aloud: [alerts and sounds](avisos-e-sons).

## Who else writes here

Nina, by voice, and the agents of this canvas. They create tasks, change the state, comment, rewrite
the text, change the deadline and delete. Every action of theirs enters the history with the name of
who did it, and their comment is what shows up on the line when they complete something. See
[the agent uses your lists](o-agente-usa-suas-listas).

In **Settings → Greeting**, **Good morning at launch** with **Mention tasks** on tells you, the first
time you open the app each day, what is overdue and what is due today across your lists.

For text you want to keep instead of do, use [the notes panel](painel-notas).
