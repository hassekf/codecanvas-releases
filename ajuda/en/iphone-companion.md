---
slug: iphone-companion
titulo: The paired iPhone
resumo: Pairing an iPhone with this Mac, revoking a device, what you can do from far away and when the phone alerts you.
area: integracoes
nivel: basico
---

In **Settings → Companion**. The phone app is called Canvas Companion, and it is part of the **Team**
plan.

## Pairing

- **Pair an iPhone**: opens the invitation window. It carries a QR code, for the phone's
  camera, and the same invitation written as a 6-character code, to be dictated.
- **Copy code**: puts the code on the clipboard.
- **The invitation is valid for 5 minutes and one use only**, and dies when you close that window. A
  clock on screen counts the time left.
- **Generate another invitation**: replaces the expired one. It is not generated on its own.
- When the phone comes in, the window replaces the QR code with the device's name.

If you paired by typing the code instead of reading the QR code, compare the characters under **This
Mac** with the ones shown on the phone. That comparison is what proves the key stored there is
this computer's.

## The device list

Each line carries the device name, when it was paired, when it last talked to this Mac and the
fingerprint of its key.

- **hasn't talked to this Mac yet**: replaces the last-seen date while the phone has not checked in.
- **chave trocada em <date>** (key changed on): appears when that device's keys have changed.
  Reinstalling the phone app and someone hijacking the account arrive here the same way.
- **Revoke**: this Mac stops accepting that device immediately, with no confirmation dialog. To come
  back, it has to be paired again, with the Mac in front of you.
- **This Mac**: shows this machine's name and the fingerprint of its key. Moving to another Mac means
  pairing the phones again.

With no device paired, nothing from outside talks to this Mac.

## What you can do from the phone

- **See the projects and each one's agents**, with the state right now, the last thing you asked and
  the files each of them wrote.
- **Read an agent's conversation**, message by message.
- **Open a file** the agent wrote.
- **See what changed** in the folder the agent works in.
- **Answer the question** that stopped an agent, picking one of the options or writing another answer.
- **Send work** to an agent. The normal send goes through the app's queue: it wakes a sleeping agent,
  waits for an open permission prompt, and can still be cancelled before it goes out. The direct send
  writes into the terminal right away, and the phone asks for one extra gesture to use it.
- **Interrupt** whoever is in the middle of something, and **dismiss** whoever is done.
- **Open a project** and switch the project in focus here on the Mac.
- **Call a new agent**, and create a work area.
- **Talk to Nina**, who answers with what she knows about this canvas.

A repeated action request does not run twice: tapping "try again" gives back the result of the first
one.

## When the phone alerts you

The phone rings in three cases: an agent **stopped to ask** (the alert carries the question itself),
an agent **finished** and an agent **crashed**. Routine state travels to the screen without ringing.

## The limits

- **The file has to be in the folder that agent works in.** Nothing outside it is reachable, and a
  large file arrives truncated, with a note saying it was truncated.
- **The list of what the agent wrote comes from the CLI's writing tools.** A file created by a
  terminal command does not enter it.
- **The Mac has to be awake.** With it asleep, the phone gets an answer saying the Mac is not ready.
- **Every command that arrives goes through the license and the device key** before becoming an
  action, and anything that deletes work asks for confirmation on the phone itself.
