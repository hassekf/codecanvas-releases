---
slug: painel-recados
titulo: Messages
resumo: Correspondence with other people running CanvasCode: contacts, what arrives, and what you can do with what arrives.
area: paineis
nivel: basico
---

Open it with `⌘K` and `recados`, `contatos`, `caixa` or `correio`. There is one panel per canvas, and
the mailbox belongs to this Mac: the same messages appear in whichever canvas you open.

Messages are part of the **Team** plan. See [license](licenca).

## Getting on someone's list

Nobody is findable by search. The link is created by invitation, in **Settings → Contacts**.

- **How you appear**: the name your contacts see. Saving changes the name for whoever already added
  you, and the screen says how many contacts now see the new name. With no name you show up as "No
  name yet" on other people's lists, and you become unreachable by name, including for Nina and for
  the agents.
- **Invite someone**: generates a 6-character code, valid for 10 minutes and for one person only.
  The invitation window replaces the code with the name of whoever came in the moment somebody redeems it.
- **I have a code**: the other side of the invitation. Type the code the person gave you.
- **The contact list**: shows the name, how many Macs that person has and the fingerprint of their
  key. The **not receiving messages** label marks whoever has CanvasCode inactive.
- **Remove**: cuts the link immediately, on both sides. To come back, one has to invite the other
  again.

The link is always mutual. Neither side sees the other's canvas, files or agents.

## When a message arrives

Two things arrive: an alert inside the canvas, which stays on screen until you act on it, and a
macOS notification. Clicking either one opens the message on top of the canvas.

An open message shows who sent it, the fingerprint of the origin key, the **signature verified** seal,
the text, the addresses mentioned in the body and the attachments.

- **Reply**: writes the reply and sends it back to whoever wrote.
- **Send to an agent**: hands the whole message to an agent in this canvas or another one, with the
  sender, the subject, the text and the files already written to disk.
- **Open an agent with this**: replaces the highlighted button when the message proposes work. The
  agent is only born when you click.
- **Archive**: takes the message off the screen and keeps it in the panel.

A message from a newer version of CanvasCode does not open: the screen says so and it stays stored
until you update.

## What you can do with what came along

| what arrived | what you can do |
|---|---|
| image | Paste into the canvas · Open in the canvas · Save as… · Send to an agent |
| text, code, markdown | Open in the canvas · Save as… · Send to an agent |
| a screen design | Import into my canvas · Save as… · Send to an agent |
| any other file | Save as… · Send to an agent |
| an address in the body | Open in the browser, or Open in media when it is a video |

Importing a design creates a new file in this canvas, with the tokens and fonts of whoever designed
it, and touches none of yours.

## The panel

- **Received**: what arrived, with a bar on the left marking the unread and the **replied** label on
  what already has an answer. Clicking a message opens it.
- **Sent**: what left this Mac, with **delivered** and to how many Macs, or the reason why the send
  did not go through.
- **The filter**: narrows the tab to one person's correspondence. It only offers names that have
  something in that tab.
- **New message**: writes a message to a contact.

## What lives where

The content is sealed on this Mac and only opens on the Mac of whoever receives it. The keys stay on
this computer, and go neither to the server nor to iCloud. Moving to another Mac means new contacts,
and the history does not come along.

When a contact's keys change, the app shows the change in the list: a reinstall and a hijacked
account arrive here as the same request, and the one who knows the difference is you.

## The agents send too

An agent lists your contacts, reads what arrived, replies to a message and sends a new one, with a
file of up to 5 MB attached. Reading a message through a tool marks it as read, and the panel stops
showing it as new. Attachments are not read by it: they come cited by name, and the one who opens
them is you. See [the agent uses your lists](o-agente-usa-suas-listas).
