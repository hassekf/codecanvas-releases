---
slug: avisos-e-sons
titulo: Alerts and sounds
resumo: CanvasCode notifications on the canvas and on macOS: which events alert you, sound and spoken alerts.
area: ajustes
nivel: basico
---

In **Settings → Notifications**.

## In the app

Notifications shown on the canvas, with CanvasCode in the foreground.

- **An agent finished**: notifies you when the agent completes the task.
- **An agent is waiting for you**: notifies you when the agent asks a question or requests a
  permission.
- **An agent crashed**: notifies you when the agent is interrupted by an error. Turning it off
  suppresses the notification and does not affect automatic recovery, configured in
  [agent settings](ajustes-agentes).
- **A task deadline is approaching**: notifies you 1 hour before the deadline, 30 minutes before and
  at the deadline. Deadlines come from the [tasks panel](painel-tarefas), and this is the only event
  with no counterpart in the next section.

Each of the four has two options:

- **Play sound**: plays a short chime along with the notification.
- **Read aloud**: the app reads the alert, only when the agent's panel is out of sight, including
  when it is in another work area. Unavailable until voice is set up in
  [setting up voice](configurar-a-voz).

## Outside the app

macOS notifications, sent only with CanvasCode in the background.

- **Notify on the Mac outside the app**: enables system notifications. When off, the controls below
  are unavailable and the app does not request the notification permission from macOS. If
  notifications don't appear after turning it on, check the permission in
  [the permissions macOS asks for](permissoes-do-mac).
- **An agent finished**, **An agent is waiting for you** and **An agent crashed**: notify the same
  events as the previous section, through macOS. Each has a **Play sound** option.

## Alert sound

- **Play sound on alerts**: turns the sound of every notification on and off, across both sections
  above. When off, no notification makes a sound and the **Play sound** options become unavailable.

## Meeting mode

During [meeting mode](agenda-e-reunioes) no notification is shown or read aloud.

## Configured elsewhere

- The voice that reads alerts: [setting up voice](configurar-a-voz).
- The panel glow when an agent finishes: [knowing what they're doing](saber-o-que-fazem).
- Announcements sent by the agents themselves: [announcements](ajustes-anuncios).
