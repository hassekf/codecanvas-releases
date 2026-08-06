---
slug: quanto-custa
titulo: What the voice costs
resumo: What spends OpenAI credits, what weighs on the conversation bill, the two ceilings and where to see the spending.
area: nina
nivel: basico
---

In **Settings → Costs**. The spending comes from the prepaid credits of the API account whose key you
saved in [Settings → Conversation](configurar-a-voz). A ChatGPT subscription does not grant API
access.

## What spends no credits

- **Dictation**: the transcription happens on your Mac. See [dictation](ditado).
- **The system voice**: it is the macOS voice, and it is the one that speaks when the natural voice
  is off.
- **The listening that opens after a spoken alert**: it uses local recognition. Staying quiet in it
  spends nothing.
- **[The written conversation](a-nina-por-texto)** (⌘J): it answers with the agent CLI you already
  subscribe to.

## What spends credits

- **The voice conversation** (⌥C): audio in and audio out. It is the most expensive item.
- **[Command mode](o-modo-comando)** (⌥X): text only, because the transcription is done on your Mac.
- **The natural voice**: the spoken alerts and the command confirmations.
- **The morning greeting**: the sentence is written by a model when there is a key; without a key,
  the app assembles the sentence itself and spends nothing.
- **Image generation and the wallpaper asked for by voice**. The chosen quality changes the price a
  lot. See [the gallery](painel-galeria).

## What weighs on the conversation bill

- **The audio she speaks** is the most expensive item of all, and it is never reused.
- **Every reply reprocesses the whole session**: the instructions, the tools and the history. The
  bill grows with the length of the conversation, not with the volume of your voice.
- **The tools you leave on take part in that reprocessing.** In **Settings → Tools**, the card at the
  top shows the approximate cost of each exchange with the current selection, and how many exchanges
  per minute fit within your account's limit; each group shows what it costs. Turning a group off
  removes its tools from the conversation and does not undo the integration.

## The two ceilings

In Settings → Conversation.

- **End after silence**: ends after this long with nobody speaking. Default 90 seconds, zero turns it
  off.
- **Maximum conversation time**: ends at the end of the time even while you are speaking, and it is
  the only one that guarantees a spending limit per conversation. Default 5 minutes, zero means no
  ceiling.

## The model

- **Nina's model**: the model of the voice conversation, and the price changes with it. The list
  comes from your account, and the "Update" button rebuilds it. The app falls back to the first on
  the list when the stored model is no longer available.
- **Command model** (Settings → Voice): the model that interprets the spoken orders.

## Where to see the spending

In Settings → Costs:

- **Spent this session**: the total of the conversation open right now, with the number of turns and
  the split between text and audio, taken from what the service charged turn by turn. The **Open the
  statement** button reveals the day's file in the Finder, kept in Application Support/codeCanvas/voz.
- **Today** and **Total**, with the number of calls beside them.
- **Last 14 days**: the chart by day.
- **By model**: calls, tokens and cost of each one. A row marked with the approximation sign is an
  estimate: the speech API reports no usage, and the value is computed from the characters spoken.
- **Clear statement**: erases the numbers from here. Charges already made remain at OpenAI.

Values below one cent are shown with four decimal places, instead of becoming zero.
