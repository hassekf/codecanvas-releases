---
slug: a-nina-por-texto
titulo: Nina in writing
resumo: The ⌘J box: what it shows, which brain answers, and how to dictate into it.
area: nina
nivel: basico
---

**⌘J** opens and closes the written conversation box, which floats above the canvas. Its settings
live in **Settings → Conversation**.

It has the same tools as [the voice conversation](falar-com-a-nina) and
[command mode](o-modo-comando), and answers about the project on your screen at that moment. What you
can ask for is listed in [what she can do](o-que-ela-consegue-fazer).

**Orders are interpreted in Portuguese**, as with the voice, so the examples below are written that
way.

## The box

- **The field**: type the request and press Enter. Anything you would say out loud works: "abre dois
  agentes do Codex", "quem está trabalhando?", "traz o Hermes de volta e manda ele rodar os testes".
- **The activity indicator**: while she works, it names what is being done at that instant, rather
  than showing a generic progress.
- **The `×` and clicking outside**: close the box. Whatever was typed in the field is still there
  next time, and a reply that was still coming keeps coming. With a dictation running, clicking
  outside only closes the box and does not reach what is behind it.
- **Esc**: closes the box.

The box never shows the reasoning nor the raw result of the tools.

## What the box shows

In the `···` menu, three modes:

- **Field only**: nothing beyond the field and the activity indicator.
- **Last reply**: the field and her last sentence. This is the default.
- **Whole conversation**: the full thread, what you sent and what she answered.

In the same menu, **See the whole conversation** opens the history in a separate window.

## Which brain answers

- **Brain of the written conversation**: picks which agent CLI answers when you write to her. It runs
  on the subscription you already have, never on OpenAI. The setting only appears with more than one
  provider enabled in Settings → Providers.

Unlike the voice conversation, this one carries on where it left off: closing the app and coming back
later keeps the same conversation.

## Dictating into it

With the box open, **⌥D** dictates into the field instead of sending to an agent. The header shows
that it is listening, and the thread that normally points at the receiving agent does not appear.

- **Dictation sends straight to the written conversation**: with this on, releasing the key sends.
  Off, the text stays in the field for you to check and press Enter. The default is to fill without
  sending. The same switch is in the box's `···` menu, named "Send when I finish dictating".

Pressing ⌥D on a canvas with no destination for the text, either because there is no agent or because
there are several and none selected, **opens the box by itself** before the first word.

## The spoken reply

- **Read the written reply out loud**: the app speaks her reply with the voice chosen in Settings →
  Voice. Off by default. In [meeting mode](agenda-e-reunioes) it stays quiet.

## What it does not do

- It does not open the microphone on its own: the input voice is dictation, and the output voice is
  optional.
- It does not read files, write files or run commands. Coding work is handed to an agent.
- It is not the conversation with an agent. Talking to a specific agent is still that agent's panel,
  or dictation. See [talking to them](falar-com-eles).
