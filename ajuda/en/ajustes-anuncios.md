---
slug: ajustes-anuncios
titulo: Announcements
resumo: Visual alerts you design and this project's agents fire when they meet a rule of yours: the fields, the placeholders, and when they reach the screen.
area: projeto
nivel: basico
---

In the [project settings](ajustes-projeto), **Announcements** section. The list belongs to each
canvas.

## The list

Each row shows the icon, the name, the style and the trigger rule, and carries:

- **The switch**: enables and disables. Disabled, the announcement stays stored and simply stops
  firing.
- **The pencil**: opens the announcement in the editor below the list. Clicking the row does the
  same.
- **The trash**: deletes the announcement.
- **New announcement**: creates an empty announcement and opens it in the editor.

## The editor

- **Name — how the agent calls it**: the announcement's key. The agent fires by saying this name,
  and a name it doesn't recognize fires nothing.
- **When to fire — the rule**: in plain language. It is the **only** field the agent reads, and the
  more specific the rule, the less it gets the moment wrong.
- **Style**: **Level Up** (center banner, three lines of text), **Pill** (at the top, two lines, the
  least intrusive) or **Achievement** (side card with the icon in a square, three lines).
- **Icon**: a grid of twelve symbols, plus a field to type any SF Symbol name.
- **Text of each part**: one field per line of the chosen style. Switching style does not erase the
  leftover text, but what is left over is not shown.
- **Test values — what the agent would fill in**: only appears when the text has placeholders. It is
  used in the simulation only, and is not saved.
- **Simulate firing**: calls the real announcement on your screen, with the test values. A
  placeholder without a test value shows its own name, and the simulation skips the wait described
  below.

## The placeholders

A stretch in braces inside the text (`{versao}`, `{quantos}`) becomes a hole the agent fills at
firing time. The placeholder name accepts letters, digits and `_`.

The template `Release {versao} no ar` becomes "Release 1.48.1 no ar" when the agent fires passing
the version. A placeholder with no value becomes empty text: the key never reaches the screen.

The agent writes nothing else. Style, icon and fixed words are yours; it says which announcement to
fire and hands over the missing values.

## When the announcement appears

The announcement enters the screen, stays about three seconds and leaves. It does **not** appear
while you are in a meeting, talking to the assistant, with the microphone open, or with the app
speaking: in those cases it joins a queue and appears as soon as you are free. None is lost.

One at a time, and the same announcement fired by several agents at once appears only once.

## What the agents receive

The list of **enabled** announcements, with the name, the rule and the placeholders to fill, goes
into the briefing of every agent in this project at the moment it is created. An announcement
created, renamed or enabled after that does not reach the agents already running.

An announcement with no name or no rule does not enter the list, even when enabled.

There is no way to ask the assistant for an announcement by voice: the agent is the one who fires
it. See [the agent works the canvas](o-agente-mexe-no-canvas).

For the alerts the app itself gives you, which are a different thing, see
[alerts and sounds](avisos-e-sons).
