---
slug: configurar-a-voz
titulo: Setting up the voice
resumo: The OpenAI key, the microphone, who speaks to you, the timbres and the voice shortcuts.
area: nina
nivel: basico
---

In **Settings → Voice**. The key and the conversation settings live in **Settings → Conversation**.

## The OpenAI key

In Settings → Conversation.

- **OpenAI key**: stores the key in the macOS Keychain. The value next to the title reads
  "configured" or "missing", and the key is never shown back to you. Saving it fetches the models
  your account actually has, for conversation and for images.

Without a key, Nina, the natural voice and the command model are unavailable. Dictation, the system
voice and [the written conversation](a-nina-por-texto) do not depend on it.

## The microphone

- **Transcription model**: picks how your speech becomes text. "Sistema (Apple)" is the default and
  shows the text while you speak. "Parakeet v3" downloads about 600 MB once and transcribes when you
  release the key. See [dictation](ditado).
- **Microphone**: picks the input device. "System default" follows System Settings and names that
  device in parentheses. A device you chose and then unplugged shows as disconnected instead of being
  swapped silently.
- **Microphone gain**: multiplies the input signal, from 1× to 24×. The default is 1×.
- **Test the microphone**: shows the audio arriving, already with the gain applied, and marks with a
  line the threshold above which speech is detected. The meter follows the gain while you drag the
  slider, and stops recording when you close Settings.
- **Audio output**: picks the output device. The app does not use this choice yet.

## Who talks to you

The three switches in this card work as a cascade: the app speaks with the natural voice; when it
cannot, with the system voice; with neither, it does not speak.

- **Nina**: turns on the voice conversation (⌥C), the morning greeting and the spoken replies to
  agents. Unavailable without the key.
- **Natural voice**: uses the OpenAI voice for alerts and for the command mode confirmation.
  Unavailable without the key.
- **System voice**: uses the macOS voice, with no key and no internet. It is the one that speaks when
  the natural voice cannot.

With all three off, the card reads "silence" and everything that would be spoken becomes an on-screen
notification. Dictation keeps working: it is transcription, not speech.

## The spoken alerts

In Settings → Voice. These apply to alerts and to the command mode confirmation, not to Nina.

- **Voice volume**: 10% to 100%, default 70%. Affects only the app's voice, not the Mac volume.
- **Alert speed**: 0.80× to 1.60×, default 1.00×. Above 1.4× the voice starts clipping the end of
  words.
- **Timbre**: picks the cloud voice. The "Listen" button plays a sample through the same path as a
  real alert, at the chosen volume and speed. Unavailable with the natural voice off.
- **Voice model**: picks the synthesis model. Unavailable with the natural voice off.
- **Command model**: picks what interprets the sentence in [command mode](o-modo-comando). It depends
  on the key, not on the natural voice: it works even with the app muted.

## Nina's voice

In Settings → Conversation. These apply only to the voice conversation.

- **Nina's model**: the conversation model. The "Update" button rebuilds the list from your account.
- **Nina's voice**: her timbre, with a "Listen" button that plays the sample without opening a
  conversation. The default is Marin.
- **Nina's speed**: 0.80× to 1.60×, default 1.00×.
- **Assistant name**: what you call her, and how she introduces herself among the agents. The default
  is Nina.
- **Silence before she answers**: how much silence she waits before assuming you are done speaking.
  From 300 to 3000 ms, default 900 ms.
- **Microphone sensitivity**: from which level upwards sound counts as speech. From 0.10 to 0.90,
  default 0.50.

## The shortcuts

The factory defaults:

- **⌥D**: [dictate](ditado) to an agent.
- **⌥X**: [tell the canvas to act](o-modo-comando).
- **⌥C**: open and close [the voice conversation](falar-com-a-nina).
- **⌘J**: open and close [the written conversation](a-nina-por-texto).
- **Esc**: cancel whatever is running, be it the dictation, the command, the conversation or the
  voice that is speaking. The text of a cancelled dictation is discarded and reaches no agent.
- **⌥F**: flip the panels and show each agent's summary.
- **⌥O**: tidy the panels with no overlap.

All of them change in **Settings → Shortcuts**: click the field on the row and press the new
combination. The screen warns when two actions end up on the same key, naming both; in that case one
of them stops working. Space is avoided in the voice shortcuts because Claude Code already uses "hold
space" to dictate inside the terminal.

The voice keys work with CanvasCode in front, including with the cursor inside an agent. With the app
behind another window, the key belongs to the app you are using. The exception is Esc, which works
across the Mac while there is voice in the air.

**While Settings is open, the voice keys do not fire.** They come back, already with the new values,
when the sheet closes, by any route.

## When you speak and nothing happens

- A signal that is too weak never crosses the detection threshold: raise the **microphone gain**
  until the test picks up your speech at normal volume.
- Room noise that never leaves silence keeps the turn from closing, and Nina does not answer: raise
  the **microphone sensitivity**. If she is cutting off the start of your sentences, lower it.
- The microphone depends on macOS permission. **Settings → Diagnostics** shows the state of each
  permission, a button that asks for it again, and one that wipes this app's permission record so the
  system asks from scratch, with the app reopened afterwards. See
  [the permissions macOS asks for](permissoes-do-mac).
