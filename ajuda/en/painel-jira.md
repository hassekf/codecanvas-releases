---
slug: painel-jira
titulo: The Jira panel
resumo: The connected project's board inside the canvas: filters, dragging cards, issue detail and the path to an agent.
area: paineis
nivel: basico
---

Open it with `⌘K` and **jira**, **board**, **issues**, **sprint**, **atlassian**, **tickets** or
**cards**. The panel only shows the board on a connected canvas; the connection is set up in
[Jira and Confluence](jira-e-confluence).

The columns are the ones from the board configured in Jira, in the same order. A project with no
software board falls back to Jira's status categories.

## The panel bar

- **The name at the top**: the name of the connection's Atlassian site, not the canvas name.
- **The project key**, next to the name: opens the list of projects this canvas's credentials can
  reach and switches the panel's project. Unavailable when the credentials reach a single project.
- **Update**: reloads the board.
- **New issue**: opens issue creation. Unavailable while no project is chosen.

## Filters and search

- **All**, **Mine**, **Bugs**: filter the cards. **Mine** matches the connected account's name;
  **Bugs** matches the issue type.
- **Assignee**: filters by one person, among those present on the board. Choosing someone while in
  **Mine** sends the filter back to **All**, and choosing **Mine** clears the assignee: the two would
  cancel each other out.
- **Show labels** and **Hide labels**: show the labels on the cards. The choice applies to every
  canvas and survives quitting the app.
- **Search**: matches the issue title and the issue key.

The quick filter and the assignee are stored with the canvas connection and come back when you reopen
the panel. The search does not: it goes away with the panel.

Every column stays visible even when a filter empties one of them. The number next to the column name
counts the cards visible in it.

## Moving and reordering

- **Dragging a card to another column**: changes the status in Jira. If the change is refused, the
  card returns to its place and an alert appears at the bottom of the panel for a few seconds.
- **Dropping a card onto another one in the same column**: reorders both in Jira. Across different
  columns, the same gesture counts as a status change.

## The card

- **Clicking**: opens the issue detail.
- **Open details**, in the **⋯** menu: the same detail.
- **Send to an agent**, in the **⋯** menu: only appears with an agent open on the canvas.
- **Copy the key**, in the **⋯** menu: copies the issue key.
- **Dragging the card into an agent panel**: types the key and the title into the agent's box
  **without** sending it, and brings the agent into focus. You finish the sentence and send. From the
  key on, the agent reads the whole issue on its own.

## The issue detail

- **Status**: becomes a menu with the transitions Jira allows there. Without transition permission it
  is a read-only field.
- **The pencil**: edits the title and the description. Only appears with edit permission. The
  description is only sent back to Jira if you touch it, so the original formatting isn't lost when
  you save only the title.
- **Attach**: uploads a file to the issue.
- **Comment**: `Enter` sends, `Shift+Enter` breaks the line. The field only exists with comment
  permission.
- **An attached image, or one embedded in a comment**: clicking enlarges it; enlarged, **Send to
  canvas** pastes the image onto the canvas.
- **A link in the description or in a comment**: asks between **Open here**, which opens a browser
  panel on this canvas, and **In external browser**.
- **Send to an agent**, in the footer: sends the mention and closes the detail.
- **Copy the key** and **Open in Jira**, in the footer: the key to the clipboard, and the issue page
  in your browser.

Changing status, commenting and editing show up on screen before Jira confirms. If the call fails,
the previous value returns and an alert says what happened.

## New issue

- **Space**: this canvas's site and project, already chosen.
- **Ticket type**: the types the project accepts, loaded from Jira when the window opens.
- **Status**: the column the issue is born in. The app creates the issue and then tries to move it
  there; with no transition available, it stays where it was created.
- **Summary**: required.
- **Description**: optional.

Once created, the card goes to the top of the column.

## When the panel has nothing to show

- **Not connected**: the **Connect Jira** button opens this workspace's settings on the Atlassian
  part.
- **No project chosen**: the **Choose the project** button leads to the same place.
- **Project with no issues**: the panel says so, and **New issue** is still available.

## Configured elsewhere

- The connection, the project and the Jira alerts: [Jira and Confluence](jira-e-confluence).
- The shortcut to the connection, inside Settings: [Integrations](ajustes-integracoes).
