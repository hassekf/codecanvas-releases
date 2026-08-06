---
slug: o-agente-usa-suas-listas
titulo: The agent uses your lists
resumo: What an agent reads and writes in your tasks, notes and messages, and what it cannot do in them.
area: agentes-fazem
nivel: basico
---

## What to ask for

- *"Check the list to see whether this is already written down before you start."*
- *"Take the next task and work on it."*
- *"Mark it done and comment on what you did."*
- *"Write the new staging token into the keys note."*
- *"Reply to Bruno's message telling him it's live."*

## Tasks

See [the tasks panel](painel-tarefas).

- **Read the list**: what is left, with deadline, state and who touched each task. Completed tasks
  only show up if the agent asks for them.
- **Create**: text and, when you name one, a deadline in `YYYY-MM-DD`, with optional time.
- **Update**: state (open, doing, done), comment, text and deadline. Only what changed is sent.
- **Delete**: the task goes to the trash, from where you restore it in the panel. The history records
  that the agent deleted it.

Three things the list doesn't show:

- **Every comment is signed with the name of the agent that wrote it.** It does not choose the
  signature, does not sign as another agent and does not sign as you.
- **Completing and deleting are different.** "It's already done" is the `done` state, with a comment
  on what was done. Deleting only happens when you ask.
- Agents are instructed not to reorder the list, not to decide priority and not to use it as a
  notebook of their own.

## Notes

See [the notes panel](painel-notas).

- **Read**: without naming one, the agent gets the titles. Naming the title or a fragment, it gets
  the whole text of that note.
- **Create**: with a title, or without, in which case the first line of the text becomes the name.
- **Update**: it appends text at the end, on a new line, or renames the note.

**There is no route for an agent to rewrite or delete what is in a note.** Deleting a note is your
own gesture, in the panel.

## Messages

Messages go to another person, on another computer. See [the messages panel](painel-recados).

- **List contacts**: whoever you have added, and whoever sent a message you haven't read. The list is
  numbered.
- **Read messages**: without naming a sender, the unread ones. **Reading this way marks them as
  read**, and the panel stops showing the message as new. Attachments don't come in the text: they
  are named, and you are the one who opens them.
- **Reply** to a message that arrived, and **send** a new one, with subject and body.
- A file can travel with the message: what goes is the content, capped at 5 MB, not the path.

Two limits:

- An agent only messages people in your contacts. Nobody is findable by search.
- **Anyone who never set their own name shows up as "no name"**, and the list number is the only way
  to address that person.
