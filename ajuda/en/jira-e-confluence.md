---
slug: jira-e-confluence
titulo: Jira and Confluence
resumo: Connecting a project to your Atlassian account, choosing the Jira project, turning the alerts on, and disconnecting.
area: integracoes
nivel: basico
---

In the project's settings, under **Integrations → Atlassian**. You get there from the project
selector, to the left of the command bar, in **Edit "<name>"…**, or from the
[Integrations](ajustes-integracoes) shortcut in Settings.

The connection belongs to each canvas: the account, the site and the token stay with that project,
and no other canvas can see them. The token is stored in your Mac's Keychain, never in an app file.

## Connecting

- **Site**: your Atlassian address, in the form `company.atlassian.net`.
- **Email**: your account's email.
- **API token**: generated at `id.atlassian.com`, under Security → API tokens. It is per site.
- **Bring Confluence along**: same token, but exposing the documentation base is a separate choice.
- **Connect**: validates the credentials. The token field is cleared after connecting.

Once connected, the **Connected** section shows the site and the account name, and says whether
Confluence came along.

## The Jira project

- **Jira project**: the menu lists the projects the credentials can reach. That project is the one
  the panel opens and the one Nina assumes when you don't say which. **None** undoes the choice.
  Next to the label, the app shows how many issues are open there.

With no project chosen, the alerts below are unavailable: there is nothing to ask about.

## The Jira alerts

Cloud Jira doesn't deliver your personal notifications to an application, so the app is the one that
asks, every so often, and only about this canvas's project. The alert is always written: a
notification on the canvas and, with the app in the background, one from macOS. Never spoken.

- **Alert me from Jira**: this project's master switch. When off, the app makes no calls at all. It
  starts off.
- **Someone mentioned you**: someone wrote your name in a comment. It's the only one that carries the
  card's key and title, and the only one that starts on.
- **A card was handed to you**: you became the assignee of a card that belonged to someone else, or to
  no one.
- **A card was created in the project**: every new card, yours or not.
- **Ask Jira every**: 5, 15, 30 or 60 minutes. The default is 15, and less than 5 isn't offered.

A project's first sweep alerts you to nothing: it marks the moment and counts from there. After a
stretch with the app closed, the app looks at the last 24 hours at most.

## What you get afterwards

- **The board on the canvas**: Jira's columns, dragging to change status, creating issues. It's the
  [Jira panel](painel-jira).
- **By voice**: *"what's on the board?"*, *"which bugs are open?"*, *"move PROJ-12 to done"*.
- **For this canvas's agents**: reading the board, opening a whole issue with its comments, creating
  and moving.
- **Searching Confluence**: only with the Confluence switch on.

The four voice tools form the **Jira e Confluence** group in Settings → Tools: turning it off keeps
the connection alive and takes Jira out of Nina's hands. On a disconnected canvas they aren't even
sent to the model.

## Disconnecting

- **Disconnect**: erases the token from the Keychain and the connection from that canvas. The voice
  tools disappear, the agents lose access, and the Jira panel has nothing to show.
