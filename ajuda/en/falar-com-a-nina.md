---
slug: falar-com-a-nina
titulo: Talking to Nina
resumo: Opening and ending the voice conversation, what closes a turn, the two clocks and the greeting.
area: nina
nivel: basico
---

**⌥C** opens and closes the voice conversation. The settings live in **Settings → Conversation**, and
the morning greeting in **Settings → Greeting**.

Nina acts on the canvas with the same tools as [command mode](o-modo-comando) and
[the written conversation](a-nina-por-texto). What she can do is listed in
[what she can do](o-que-ela-consegue-fazer); the tool groups are turned on and off in Settings →
Tools.

**The voice command understands Portuguese.** The app interface speaks English, Portuguese and
Spanish, and dictation follows the chosen language, but spoken orders are interpreted in Portuguese.

## Opening and ending

- **⌥C**: turns the conversation on and off. It is a switch, not a push-to-talk.
- **"Pode dormir"**, "tchau", "valeu", "chega": ends the conversation. She does not say goodbye; the
  silence is the confirmation. The agents keep working.
- **Esc**: cuts the conversation and the speech in progress, with the app in any window.
- **Confirm on activation**: makes Nina say one word when the microphone opens. Off, the first thing
  in the conversation is your voice.
- **Opening word**: changes that word. Left blank, the default word for the active language applies.

When the conversation is woken by an alert, she skips the opening word and starts out already knowing
which agent it was about.

The voice conversation keeps nothing from one session to the next: once ended, the next one starts
without what was said before. What does keep memory are the agents, and
[the written conversation](a-nina-por-texto).

## During the conversation

- Starting to speak interrupts Nina mid-sentence.
- The turn closes on **silence**, never on the length of your speech. How much silence counts as the
  end is **Silence before she answers** (default 900 ms), and from which level sound counts as speech
  is **Microphone sensitivity**, both in Settings → Conversation.
- The window frame lights up while she speaks.
- While the conversation is running, the media panel is muted.
- The conversation does not open in [meeting mode](agenda-e-reunioes): ⌥C shows a notification saying
  the microphone belongs to the call, with the exit button next to it.

### The two clocks

- **End after silence**: ends the conversation after this long with nobody speaking. From 0 to 300
  seconds, default 90. Zero turns it off.
- **Maximum conversation time**: ends at the end of the time even while you are speaking, and it is
  the only one that guarantees a spending ceiling. From 0 to 30 minutes, default 5. Zero means no
  ceiling. In the last minute the voice window shows the countdown.

## When the app speaks first

An agent that finishes, that asks a question or that crashes produces an alert, and the app speaks it
if any voice is on. Which events alert you, with sound and with speech, is in
[alerts and sounds](avisos-e-sons).

- **Answer agents by voice**: after the spoken alert, the app opens the microphone for a few seconds
  so you can reply out loud. Off, it only alerts.
- **Response window**: how long that listening lasts, from 0 to 15 seconds, default 6. Zero turns the
  listening off. It uses local recognition and spends no credits.

What you say in that window decides what happens:

- **"Me leva lá"**, "abre o painel dele", the agent's name: takes you to it, switching project and
  workspace if needed.
- **"Depois"**, "beleza", "deixa pra lá": closes the listening without doing anything.
- **"Continua"**, "tenta de novo", "pode mandar": tells the agent to resume. Only valid right after a
  crash alert.
- **"Só quando voltar ao ar"**: waits for the provider to come back before resuming. Only valid right
  after a crash alert.
- **Any other sentence**: wakes the conversation, already knowing which agent the alert was about. A
  single word the app does not recognise sends the whole sentence to the conversation, which is why
  an answer meant for an agent ("pode ir de Postgres") is never mistaken for a navigation command.

Staying quiet closes the window without spending anything.

## The morning greeting

In Settings → Greeting.

- **Good morning at launch**: the app tells you how the day looks the first time you open it that
  day, and only when something is pending. With Nina on, the greeting becomes a conversation; with
  her off and some voice on, it is a spoken message; with no voice at all, it is an on-screen
  notification.
- **Mention tasks**: includes what is overdue and what is due today in your lists.
- **Mention meetings**: includes today's appointments, if [the calendar](agenda-e-reunioes) is
  connected.

Below the switches, the **Today** section shows what it would talk about if you opened the app right
now, project by project. With nothing pending in any project, it says nothing.

Each of the two content switches warns you when the matching tool group is off in Settings → Tools:
Nina mentions the task or the meeting, but cannot act on it by voice.
