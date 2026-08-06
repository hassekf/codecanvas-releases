---
slug: agenda-e-reunioes
titulo: Calendar and meetings
resumo: Connecting the Mac calendar, what Nina may see of it, the alert before the hour and meeting mode.
area: integracoes
nivel: basico
---

In **Settings → Integrations**. CanvasCode reads the Mac Calendar, with every account already in it,
and never writes anything to your calendar.

## Connecting

- **Connect the calendar**: turns the integration on. macOS asks for permission at that moment. If
  permission is denied, the switch goes back to off, and the section shows a button that opens Privacy
  and Security → Calendars in System Settings, because macOS will not ask again on its own.

Once on, the section shows how many appointments there are today. Off, the integration leaves no trace:
no block on the start screen, no alerts, and Nina receives nothing on the subject.

- **Which calendars are included**: ticks and unticks each Mac calendar. None ticked means all of
  them.

## What Nina may see

Five items, on by default, deciding what is uploaded to OpenAI when you ask Nina about the calendar:

- **The title**: without it, she only knows an appointment exists.
- **The location**: the room, the address, the building.
- **The description and agenda**: the body of the invitation.
- **The attendees**: who was invited and who accepted.
- **The call link**: the Meet, Zoom or Teams address. Without it she cannot open the call by voice.

The time always travels with the appointment, whatever you tick. The alerts, the block for the day
and the on-screen notifications are assembled on your Mac and do not go through OpenAI, regardless of
these five.

The whole calendar tool group can also be turned off in Settings → Tools: Nina then stops reading the
calendar and joining calls, and the integration stays connected.

## Your day on the start screen

Below the projects there is a block with today's appointments, or tomorrow's when today has none
left. The header says which of the two days is being shown.

- What is past stays in the list, dimmed; what is happening is marked as "agora".
- Hovering over a meeting with a link shows the join button.
- Clicking the row opens the detail: time, source calendar, attendees, agenda and an **Open in
  Calendar** button, which is where appointments are created, moved and cancelled.

## The alert before the hour

- **Alert before the meeting**: shows a notification before the meeting starts. It does not disappear
  on its own.
- **Notify beforehand**: how many minutes before, among 5, 10, 15 and 30. The default is 10.

The alert is about one meeting at a time, always the next one that has not started. For a meeting
with a link it offers both ways to join, the one you prefer first and the other next to it, plus a
button that dismisses it. The alert leaves on its own an hour after the meeting ends, or the moment
it is cancelled in the calendar.

- **When opening a meeting**: chooses between "In a panel here" and "In my browser". Here inside,
  Meet opens with the Google session the browser panels already use.

When you join through a panel here, the call becomes the focus of the screen if the canvas arranges
itself. With the panels arranged by hand, nothing is moved.

## Meeting mode

Joining a call from the alert, by voice or from the button turns meeting mode on. While it is on:

- Nothing is spoken and no notification appears.
- The microphone does not open by itself after an alert.
- **The dictation, command and conversation keys do not open the microphone.** Pressing one of them
  shows a notification saying the microphone belongs to your meeting, with the exit button next to
  it.
- A voice conversation that was open is ended as you join.

The badge on the bar reads "In a meeting" and is the way out: clicking it turns the mode off. The mode
also leaves on its own five minutes after the appointment ends, and leaves when you close the panel
the call had opened in.

By voice, "fica quieta um pouco" turns the mode on with no meeting at all, and "acabou a reunião"
turns it off.

### Nothing is lost

Whatever would arrive during the meeting is kept. On the way out, alerts describing a problem that is
still alive, such as a crashed agent, come back in full; the rest become one notification saying how
many arrived, with a **View** button that opens the history.

## By voice

```
"o que eu tenho hoje?"           "qual a próxima reunião?"
"do que é a reunião das três?"   "quem vai estar nela?"
"entra na reunião"               "abre o Meet"
"fica quieta um pouco"           "acabou a reunião"
```

The orders are interpreted in Portuguese. Without saying which one, she joins the meeting happening
now or the next one to start. There is no way to create, move or cancel an appointment by voice.

## In the morning greeting

- **Mention meetings** (Settings → Greeting): includes today's appointments in the morning greeting,
  in the same sentence as the other pending items. See [talking to Nina](falar-com-a-nina).
