---
slug: ditado
titulo: Dictation
resumo: ⌥D and speak: where the text goes, what becomes a symbol, the two engines and long-form dictation.
area: nina
nivel: basico
---

**⌥D** dictates to an agent. The key changes in **Settings → Shortcuts**, on the "Ditar" row, and the
transcription engine is chosen in **Settings → Voice**.

The text reaches the agent word for word, with no model rewriting what you said.

## The key

- **Hold and release**: the app listens while the key is held; releasing sends.
- **Tap and release**: listening stays latched and you can speak freely. The small window then reads
  "tap again to send", and that tap is what sends.
- **Esc**: cancels. The text is discarded and reaches no agent.

With listening latched, one minute of silence pauses the dictation. What you said is kept in a notice
with three ways out: **Keep talking**, **Send** and **Discard**. With no agent chosen, the notice asks
you to click the panel of whoever should receive it, and sending stays unavailable until then.

## Where the text goes

The rules are fixed, with no model deciding:

- **"Peça pro Marshall extraia o guard clause pro topo"**: goes verbatim to Marshall. Several ways of
  addressing are recognised ("peça pro", "pede pro", "manda pro", "fala pro", "diz pro", "ei"), and
  the name and the connectors at the start are stripped from the text.
- **"Foco no Marshall"**: highlights his panel, sending no text.
- **Any other sentence**: goes to the selected agent. With a single agent on the canvas, it goes to
  that one.
- **With [the written conversation](a-nina-por-texto) open**: lands in its field.

The name is matched ignoring accents and case. The dictation window shows the destination next to the
text, or "sem destino" when there is nobody to send to. **A file selected on the canvas travels with
the text**, as a reference in front of what you dictated, and the window marks that next to the name
of the receiving agent.

- **Dictation thread** (Settings → Interface): turns on the thread that runs from the dictation bar to
  the panel that will receive the text. Off, the destination is still written next to the bar.

## Dictated punctuation

Four words become symbols when they sit between two pieces that look like an identifier:

- **"underline"** and **"sublinhado"** become `_`.
- **"barra"** becomes `/`. "Src barra components" becomes `src/components`.
- **"hífen"** becomes `-`.
- **"ponto"** becomes `.` only before a known file extension. "Index ponto tsx" becomes `index.tsx`;
  "até que ponto é viável" stays as you said it.

The conversion does not happen when either side is an ordinary word, as in "na nossa barra aqui
embaixo". Beyond that, dictation does not touch your punctuation and does not correct your text.

## The two engines

In Settings → Voice → Transcription model.

- **Sistema (Apple)**: comes with macOS and shows the text while you speak. It is the default.
- **Parakeet v3**: downloads about 600 MB, once, from the button on the card itself, and runs on your
  Mac with no internet. It transcribes when you **release** the key: while you speak the window reads
  "ditando…", and the text arrives at the end.

Dictation follows the language chosen for the app. What still understands Portuguese only are the
spoken orders of [command mode](o-modo-comando).

## Long-form dictation

In **Settings → Diagnostics**, four switches that apply only to Parakeet and only to speech longer
than about fifteen seconds. All of them start on.

- **Avoid language switching**: keeps the text from slipping into English in the middle of
  Portuguese.
- **Recover lost passages**: rebuilds words swallowed at the seam between dictation windows.
- **Split long speech into pieces**: cuts the audio at the silences and transcribes each piece
  separately. It makes long speech slightly slower.
- **Anchor the language in each piece**: puts a word of the language in front of each piece and
  removes it from the final text.

## Sending it again to another agent

```
"aquilo da migração, joga pro Hermes"
"mandei errado, reenvia o último pro Apolo"
```

The app finds what you already dictated in the history and delivers it to the other agent, without
you repeating the sentence. It is a voice request, so it works through ⌥C or ⌥X.

## Limits

- Dictation and conversation compete for the same microphone: opening the conversation while the
  dictation key is held is refused, with a warning.
- In [meeting mode](agenda-e-reunioes) dictation does not open the microphone, and the app shows a
  notification saying it belongs to the call.
