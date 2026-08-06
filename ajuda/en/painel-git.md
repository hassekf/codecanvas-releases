---
slug: painel-git
titulo: The Git panel
resumo: The repository's three tabs: what is in your folder, the issues and the pull requests, with what each button does.
area: paineis
nivel: basico
---

The project repository in three tabs: **Git**, **Issues** and **PRs**. Each tab shows how many items
it holds; when the count is zero, no number appears.

Open it with `⌘K` typing "git", or by clicking the branch indicator in the footer. The panel is one
per canvas: asking again brings the existing one to the front.

## The footer indicator

- **The current branch**, truncated in the middle when it is long.
- **Arrows**: how many commits you are ahead of and behind the remote. They appear only when there
  is divergence.
- **The count of changed files**, with the total lines added and removed, or the word "clean" when
  there is nothing to commit.
- **"N contested"**, when some changed file has more than one author.
- **Clicking** opens this panel.

## The Git tab

The header carries the branch, the divergence arrows, the pull request badge for this branch and the
reload button. With no remote configured, the arrows do not appear. Outside a repository, the tab
says the workspace is not a git repository.

- **Changes**: the files modified and not yet committed. Each row carries the status letter, the
  path, how many lines went in and out, and the name of whoever touched the file, including before
  any commit. Your own edit in a [file panel](painel-arquivo) counts as authorship.
- **Contested file**: one with two or more authors gets an alert on its row. The list is ordered
  conflicts first, contested files next, and the rest by path.
- **Commits**: the last 25, with summary, author and when. A commit created by an agent in this
  session shows the agent's name; the rest show the author recorded by git, which is you in all of
  them.
- **Diff**: clicking a changed file opens the diff in place of the list. The arrow in the top corner
  goes back.

## The Issues tab

The repository's open issues.

This tab's buttons are labelled in Portuguese, whatever language the app is in.

- **The filter at the top** narrows by label. **All issues** turns the filter off.
- **Clicking an issue** expands the actions, the labels and the description.
- **Trabalhar nisto** ("work on this"): opens a new agent with the issue set up as its first task.
  With more than one provider enabled, the button becomes a menu of which one to open.
- **Mandar para…** ("send to"): hands the same task to an agent already open on this canvas. With no
  agent open, the button does not appear.
- **Fechar** ("close"): marks the issue as resolved on GitHub.
- **Abrir no app** opens the issue in a [browser panel](painel-navegador); **Abrir no GitHub** opens
  it in the system browser.

The text delivered by **Trabalhar nisto** and by **Mandar para…** is the same, and it instructs the
agent to comment on and close the issue itself when it is done.

## The PRs tab

The open pull requests.

- **All** and **Awaiting you**: the second one narrows to those stuck on your review.
- **Collapsed**, each row carries number, title, the review badge (**Approved**, **Changes**,
  **Awaiting**) and the CI badge, when the PR has CI.
- **Clicking** expands it, and only then does the app fetch the description and the files, which the
  listing does not carry.
- **Approve**: asks for confirmation and publishes the approval on GitHub. It is unavailable on a PR
  you have already approved.
- **Comment**: opens a text field. **Send** publishes a standalone comment, which does not become a
  review.
- **The changed files** appear with each one's line balance. Clicking any of them opens the PR's
  files in the browser.

Merging and requesting changes do not exist in this panel.

## The pull request badge

When an agent's branch has become a PR, its number and the CI state appear on the agent's panel, in
the footer and in the Git tab header. With no open PR, the badge takes up no space.

The switch is **Pull request badge**, in [agent settings](ajustes-agentes). When off, no badge
appears and the app stops asking GitHub about your PRs.

## What the Issues and PRs tabs require

They talk to GitHub through `gh`, its command line tool, using the login already set up there. When
something is missing, the tab says which of the three it is: `gh` not installed, `gh` not logged in,
or the project with no GitHub remote.
