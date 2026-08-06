---
slug: worktrees-e-isolamento
titulo: Each agent in its own copy
resumo: Isolation by worktree, the text that instructs the agents, the workstreams sidebar and handing off a finished workstream.
area: agentes
nivel: avancado
---

## The isolation

In **Settings → Agents → Isolation by worktree**, on by default.

- **Isolation by worktree**: instructs each agent to create its own worktree of the repository and to
  commit on its own branch before writing any file. When off, every agent writes in the same
  directory.
- **The instruction applies to the next agents.** It goes into the system prompt when the process is
  born, and no agent already running changes behaviour when you save.
- **It is an instruction, not a lock in the app.** An agent chooses to follow it, and the protocol
  skips the worktree for read-only tasks and for projects with no Git repository.

## The text the agents read

- **Customize instructions…**: opens the protocol editor, right below the switch. Once edited, the
  button reads **Edit instructions…**.
- **{nome}**: the marker that becomes each agent's identifier, and therefore its branch and its
  folder. Without it the editor warns you and still allows saving, and the agents fight over the
  same branch.
- **Restore default**: puts the factory text back in the editor, and is unavailable when what is
  there is already the default.
- **Complete** with the text empty, or identical to the default, undoes the customization: the
  project goes back to following the default text instead of keeping a copy of it.

Each project can disagree with the app-wide setting, in **Edit the project → Agents → Isolation by
worktree**:

- **Follow the global setting**, **On in this project** or **Off in this project**.
- **This project's own instructions**: appears with the isolation on, and replaces the global text on
  this canvas only.

## The workstreams sidebar

`⌘⇧F` opens and closes the sidebar on the left. The key is changed in Settings → Shortcuts.

Each section is a work area, including the ones out of sight, and inside it comes one row per agent.

- **A workstream row** brings the agent's name, the lines added and removed, the branch, the stage
  and how many commits from the destination it has not seen yet. Clicking it takes the camera to the
  agent.
- **The "branch only" tag** marks work that exists as a branch and no longer has a directory.
- **Agents with no workstream also appear**, with their current state: whoever only read code has
  neither branch nor worktree.
- **The top row** is the canvas base, with how many files are uncommitted there.
- **The eye in the header** shows and hides the subject each agent noted down.
- **The button beside it** switches between the floating sidebar and the sidebar docked to the side,
  with the canvas next to it. It is born floating.
- **The contested files** sit at the foot of the list: the ones more than one workstream is touching
  right now, committed or not.
- **The footer** counts how many workstreams are ready to merge and how many are under review, and
  the button beside it re-reads the repository from scratch, using nothing it already knew.
- **A large repository is not read whole.** Branches with a worktree always come in, and from the
  rest the most recent ones do. The sidebar says how many were left out.
- **A row's context menu** goes to the agent, or brings an agent into an ownerless worktree, and
  copies the worktree path, the branch name, or opens the folder in Finder.

## What the sidebar lists

In **Settings → Interface → Workstreams sidebar**.

- **Show branches without a worktree**, on: branches whose working directory has already been removed
  also appear. When off, a branch in that state is invisible.
- **Show the already merged ones**, off: workstreams already whole in the base leave the list.
- **Hide the area tabs while it's docked**, off: the tabs at the top disappear and the sidebar takes
  over switching areas, renaming and creating. It only works with the sidebar docked, and is
  unavailable while it is floating.
- **Group the agents into tabs**: in an area with more than one agent, they share a panel with tabs
  at the top. Each area's context menu can decide on its own.

## Handing off a workstream

The handoff button appears on the row of workstreams that are ready, published or under review, and
on the others only when the cursor is over them.

- **The button merges nothing**: it sends a message to the agent inside that worktree.
- **The label names the destination** inferred from the branch's own history: merge into that branch,
  open a pull request to it, or just say it's done.
- **The button's menu** changes the mode. The choice applies to that destination and is remembered.
- **Resume**, on stopped or empty workstreams with nobody inside: opens a new agent and sends it into
  that worktree. The button does not appear when the workstream already has an agent.

In **Settings → Interface**:

- **How to hand off a finished workstream**: picks the default mode for every destination of every
  project. Infer from each destination looks at how work entered that branch before and suggests the
  same. The choice made in the sidebar menu overrides it, and only for that destination.
- **Edit the message…**: rewrites the text the button sends. The three markers become the branch
  name, the destination and the verb of the chosen mode, and without the action marker the message
  does not say what to do.

## When several finish at the same time

An agent that has just merged can pass the turn to the next one in line, and the next one gets a
notice in its panel that its turn has come. This only reaches agents alive on this canvas: one that
was dismissed or is on another canvas is not woken.

## Configured elsewhere

- The work areas that become the sidebar's sections: [work areas](areas-de-trabalho).
- The state of each agent: [knowing what they're doing](saber-o-que-fazem).
- The repository on the canvas: [the agent and the repository](o-agente-e-o-git).
