---
slug: o-agente-e-o-git
titulo: The agent and the repository
resumo: Reading repository state with authorship for uncommitted files, resolving issues and reviewing GitHub pull requests.
area: agentes-fazem
nivel: avancado
---

## What to ask for

- *"Before you touch that file, check whether anyone else is in it."*
- *"Tell me what hasn't been committed and what each one has been changing."*
- *"Take the first issue and fix it. Comment the cause and close it once the fix is committed."*
- *"What is waiting for my approval?"*
- *"Read PR 214 and tell me whether it can be approved."*

## Reading the repository

An agent reads the current branch, what hasn't been committed and the latest commits.

**Along with it comes what git does not have: which agent wrote in each dirty file.** Git history
only knows commits, and a changed, uncommitted file has no author at all. CanvasCode records
authorship for edits made by this canvas's agents, and the reading flags when two agents are in the
same file.

- There is no conflict for git to detect in that case, because nothing was committed. Whoever saves
  last overwrites the other.
- The same report is available to you in [the Git panel](painel-git).
- The way out for heavy parallel work is one agent per copy of the project, in
  [worktrees and isolation](worktrees-e-isolamento).

## GitHub issues

- **List** open issues: title, labels and preview. A label filter narrows the list.
- **Read a whole issue**, with the full body, by number.
- **Comment**, **rename** and **close**, with an optional closing comment.
- **Reopen** a closed issue, with the reason.

Agents are instructed to comment the real cause rather than just "fixed", to rename the title when it
only describes the reported symptom, and to close once the fix is committed or once they conclude it
was not a bug.

Jira issues are a different thing, and live in [the Jira panel](painel-jira).

## Pull requests

- **List** open PRs: title, author, branch, review state and CI state.
- **Read a whole PR**, with the description and the changed files, by number.
- **Filter** to the ones requesting your review.
- **Approve**, publishing an approval review on GitHub, with an optional comment.
- **Comment**, without approving.

**Requesting changes and merging do not exist here.** Merging remains yours, or the agent's in its
own terminal.

## What this requires

Issues and pull requests come from GitHub through `gh`, with the login already on the machine. When a
piece is missing, the agent is told which of the three it is:

- `gh` is not installed;
- `gh` is installed and nobody has logged in;
- the project has no GitHub remote.

## What does not exist here

- Committing, creating branches and merging are not canvas actions. The agent does that in its own
  terminal, as it would outside the app.
- An agent sees the repository of the project it lives in, and only that one.
