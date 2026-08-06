---
slug: ajustes-integracoes
titulo: Integrations
resumo: The Mac calendar in Settings, what Nina sees of it, and why Jira is connected in the project's settings.
area: ajustes
nivel: basico
---

In **Settings → Integrations**.

## The Mac calendar

- **Connect the calendar**: brings in the events from every account your Mac already has, including
  iCloud, Google and Exchange. The app only reads the calendar; it never writes anything into it. When
  you turn it on, macOS asks for permission. If you deny it, the switch goes back to off.
- **macOS denied access**: appears under the switch when permission was denied. macOS won't ask again
  on its own, and **Open System Settings** takes you to the Calendars screen. The other permissions
  are in [the permissions macOS asks for](permissoes-do-mac).

When off, the calendar doesn't exist for the app: nothing on the home screen, no alerts, and Nina
doesn't get the calendar tool.

When on, the controls below appear.

- **What Nina can see**: five switches, one per piece of an event (the title, the location, the
  description and agenda, the attendees, and the call link). Only what is on goes up to OpenAI, and
  only when you ask Nina about your calendar. The events shown on the app's screen never leave your
  Mac. The call link is what she needs to open a meeting by voice.
- **Which calendars are included**: one switch per calendar your Mac has, with each one's account.
  None checked means all of them; the first uncheck materializes the list.
- **Alert before the meeting**: the alert appears before the start and stays until you join or dismiss
  it.
- **Notify beforehand**: 5, 10, 15 or 30 minutes before. Only appears with the alert on.
- **When opening a meeting**: **In a panel here**, which opens the call in a canvas browser already
  signed in to your Google account, or **In my browser**. You can switch on the spot, in the alert
  itself.

What happens on the day of the meeting is in [calendar and meetings](agenda-e-reunioes).

## Atlassian

Jira and Confluence are not connected here: the connection belongs to each canvas.

- **Jira for "<project name>"**: with a project open, the **Connect** or **Edit** button opens that
  workspace's settings already on the Atlassian part. The text next to it says whether it is already
  connected.
- **No workspace open**: with no project open there is nothing to connect, and the screen says so.

The step by step is in [Jira and Confluence](jira-e-confluence).

## Where the secrets live

Every integration credential is kept in your Mac's Keychain, never in an app file, and disconnecting
erases the credential with it.
