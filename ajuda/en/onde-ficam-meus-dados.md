---
slug: onde-ficam-meus-dados
titulo: Where your data lives
resumo: What CanvasCode keeps on your machine, where it keeps the secrets, and what leaves here, for where and because of what.
area: conta
nivel: basico
---

CanvasCode has no account and no data server of its own. What leaves your machine leaves because a
feature you used needs an outside service, and this page says which one, and what.

## On your disk

In `~/Library/Application Support/codeCanvas`:

- **`canvases.json`**: the projects, the panels with position and size, the work areas, the theme,
  the background, the saved arrangements and the record of the agents that lived in each project.
- **`tarefas/` and `notas/`**: tasks and notes, one file per project.
- **`imagens/`**: the generated and pasted images, one folder per project, with the prompt that
  created each generated one.
- **`fundos/`**: a copy of every wallpaper you chose or asked for.
- **`modulos/` and `modulos-dados/`**: the modules you created and what they store.
- **`voz/`**: the voice usage statement, one file per day, and the technical log that records every
  microphone connection.
- **`custos/`**: the record of what voice and conversation spent.
- **`Recados/`**: the messages already opened, the ones you sent and the confirmation queue.
- **`entregas/`**: what one agent writes for another when one of them delegates a task.
- **`backups/`**: automatic copies of `canvases.json`, the preferences, the tasks and the notes.
- **`crashes.json` and `quedas.jsonl`**: the record of app crashes and of agent failures.

**Screen recordings** go to `~/Movies/codeCanvas`. The app's **preferences** live where macOS keeps
app preferences.

None of this is sent anywhere, and the backups do not leave the machine either.

## The secrets

They live in the **macOS Keychain**, never in a text file:

- your OpenAI key;
- your license key and the token activation returns;
- the tokens of the integrations you connect, one per project;
- the secrets you enter for MCP servers;
- this Mac's private keys for messages.

The OpenAI key field shows whether it is configured, never the key itself. The backups carry none of
these items.

## The agents' conversation

It belongs to the agent program, not to the app, and lives in that program's folder: `~/.claude`,
`~/.codex` and equivalents, or the folder of the account you chose for that project. CanvasCode keeps
only the **key** of each conversation, which is what lets you recall an agent with its whole memory.

An agent recalled under a different account does not find the conversation it had under the first
one. See [accounts and profiles](contas-e-perfis).

## What leaves here

### The agents

What you send an agent goes to that agent's service, exactly as it would if you ran the same program
in your terminal. The app does not sit in the middle of that conversation and keeps no copy of it.

### Voice, commands and images

All of this uses your OpenAI key, and none of it happens without one.

- **The conversation with the assistant** sends and receives **audio**.
- **The voice it speaks with** sends the text to be read.
- **Command mode** sends **text**: the transcribed phrase, plus the names of the live agents, the
  open projects, the themes and the enabled CLIs. With no key, it uses the model that runs on your
  Mac.
- **Generating an image** and **asking for a wallpaper** send your request. The wallpaper's "search"
  looks on the web through OpenAI's service.

**Dictation** does not leave the machine with either engine: the system one transcribes through
macOS, and Parakeet runs on your Mac after downloading the model. See [dictation](ditado) and
[what it costs](quanto-custa).

### The calendar

The calendar is only read if you turn it on in **Settings → Integrations**. Once on, five items of
each event can be sent to the assistant along with the conversation, and you choose them one by one:
title, location, description and agenda, attendees and call link. All start on. You also choose which
Calendar calendars are included. See [calendar and meetings](agenda-e-reunioes).

### The messages

A message leaves this Mac encrypted end to end, with keys that exist only in the Keychain here and in
the recipient's. The server delivers and forgets the envelope; the copy that remains is the one on
your disk. See [the messages panel](painel-recados).

### Company integrations

Jira and Confluence talk to your organization's server, and only when you ask. See
[Jira and Confluence](jira-e-confluence).

### The license

Activating, revalidating and releasing the Mac send your license key, a **code derived from this
Mac's identifier**, and the Mac's name as macOS knows it. Activation also sends the app version and
the macOS version. The Mac code is scrambled and cannot be reversed. See [license](licenca).

### Crash reports

When the app crashes, macOS writes a technical report on your disk. The **Send crash and
failed-resume reports** switch, in **Settings → Diagnostics**, decides whether it is sent; the app
asks the first time there is anything to send.

- The report carries the trace of where the app stumbled, its version and the macOS version. It does
  **not** carry your code or your files.
- The same switch covers the failure where an agent comes back without its conversation. That sends
  counts, dates and the session identifiers; your project path becomes a code, and the names of your
  accounts do not leave here.
- With it off, nothing is sent. The list below the switch shows what has been collected and what is
  still to send, with a send button on each row.

### Updates

The app asks the update server whether there is a new version and downloads one when there is. Every
update is signed, and the app refuses any file whose signature does not check out. See
[updates](atualizacoes).

## The agents talk to the canvas without leaving the machine

When an agent opens a panel, reads your tasks or takes a picture of the browser, it talks to a server
the app starts inside your Mac. It listens on loopback only, and it requires a secret that is born on
each app run and handed to each agent born here.

## Taking everything with you

The app's folder is an ordinary folder: you can copy it, keep it or delete it from Finder. Outside it
are the secrets in the Keychain, the recordings in `~/Movies/codeCanvas`, and the agents'
conversations, which belong to their own program.
