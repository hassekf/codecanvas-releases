---
slug: painel-elenco
titulo: The cast panel
resumo: This project's agents in four sections, what the search reaches, and what each button does to a stored agent.
area: paineis
nivel: basico
---

This project's agents in a list, the ones on screen and the ones already dismissed. Open it with
`⌘K` typing "elenco", the name it goes by in the panel catalog. The panel is one per canvas.

The list belongs to the project: every canvas has its own cast. The agents running the steps of an
[Initiative](painel-iniciativas) do not appear here.

## The four sections

Each one carries its count in the header.

- **On screen**: the agents open and awake, with the state light and what each one is doing.
- **Hibernating**: the open agents that went to sleep after being idle. They stay on the canvas and
  wake up when they get a prompt. What controls this is **Hibernate idle agents**, in
  [agent settings](ajustes-agentes).
- **Stored**: the dismissed agents that have a conversation to resume, with the last mission in
  quotes and how long ago they were active.
- **Stored without history**: the dismissed ones that never got a task. They only hold a name.

With no agent at all, the panel says the project has none yet; with the search filled in and no
result, it says nothing was found.

## The search

The field at the top filters all four sections at once. It looks at the name, the mission, the
subject and the summary the agent noted, its pending item, and **every delivery** it recorded,
including those of agents already dismissed.

When what matched the search was an old delivery, that delivery appears on the row itself, with how
long ago it happened. The same search works by voice: *"who worked on payments?"*.

## The buttons on each row

- **Go to the panel** (in the On screen section): selects the agent and takes the camera to it.
- **Call** (in the stored sections): reopens the agent with its whole conversation. It comes back
  with the same name and the same history.
- **Forget** (in the stored sections, on hovering the row): removes the agent from the cast and
  frees its name. It asks for confirmation, and there is no undo.
- **Clicking the row** opens the summary.

Stored agents also show up in `⌘K` when you type their name, and picking one there is the same as
pressing **Call**. They appear in [search](busca-e-comandos) only when looked for.

## The opened row

- **What the agent noted**: the subject, the summary and the pending item, when it recorded any.
  With no summary noted, the mission appears; with neither, the panel says it has not noted anything
  yet.
- **Delivered**: the timeline of what it has delivered, most recent first, with how long ago each
  one was. It shows the last six and sums up the rest in one line.

This is the only place where the history of a **dismissed** agent appears. To follow the ones on
screen, see [knowing what they're doing](saber-o-que-fazem).

## Clearing the sections

- **Forget all**, in the **Stored** header: forgets every agent that has a conversation. It asks for
  confirmation twice.
- **Free up names**, in the **Stored without history** header: forgets them all at once, with a
  single confirmation.

In both cases the names become available to new agents, and there is no way to call back whoever was
forgotten.
