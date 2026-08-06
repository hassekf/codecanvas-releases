---
slug: criar-e-fechar
titulo: Creating and closing agents
resumo: Opening an agent, dismissing it, calling it back with its conversation, forgetting it for good, and what happens when it sleeps or crashes.
area: agentes
nivel: basico
---

## Creating

- **The new agent button, on the command bar**: opens the **New agent** dialog.
- **`⌘N`**: creates a Claude Code straight away, with the cursor already inside it, even while you
  are typing to another agent. **`⇧⌘N`** creates a Codex, and only works with Codex enabled in
  **Settings → Providers**. Both keys can be changed in **Settings → Shortcuts**.
- **`⌘K`**: the new agent entries, one per enabled CLI, create the agent directly, with no dialog.
- **By voice**: *"open an agent"*, *"start three agents"*. Saying the name of an agent that already
  exists never creates another one, even if that agent is stored.
- **An agent**, when it brings colleagues onto the canvas. See
  [one agent calls another](um-agente-chama-outro).

## The New agent dialog

- **Tool**: which CLI the agent is born in. Only appears with more than one enabled.
- **Account**: which installation it is born in. Only appears if there are accounts registered for
  that CLI, and it goes back to **The project's** when you switch tools. See
  [accounts and profiles](contas-e-perfis).
- **Name**: comes with a suggestion. Clicking the field clears the suggestion, and confirming with an
  empty field uses it anyway.
- The folder is shown below and is not editable here: it is the canvas folder.

## Dismissing

Closing an agent panel, with the close button in the header or with the Delete key while the canvas
has focus, ends the process and takes the panel off screen. The project keeps the name, the CLI, the
account, the last task, the subject the agent wrote, the deliveries and the key to the conversation.

## Calling back

- **In the cast panel**, with the **Call** button. See [the cast panel](painel-elenco).
- **In `⌘K`**, by typing its name.
- **By voice**: *"call Hermes back"*. Sending a task to a stored agent also brings it back.

It returns in the same CLI and the same account it was born in, and the conversation carries on from
where it stopped.

### When the conversation isn't found

- An agent that **never received a prompt** has no conversation recorded, and the app says nothing:
  it comes back new.
- An agent that **has already talked** and whose conversation isn't found produces an alert naming
  the account the app looked in.
- If the conversation is in **another registered account**, the alert says which one, and switching
  that agent's account is what brings it over. The app never copies anything between accounts on its
  own.

## Forgetting

Forgetting is the opposite of dismissing: the agent leaves the cast, can no longer be called back and
its name becomes available again. The conversation folder stays on disk.

**Forgetting only happens in the [cast panel](painel-elenco)**, not in the agent's own panel. There:

- **The forget button**, on each stored row.
- **Forget all**, in the header of the **Stored** section, asks for two confirmations, because those
  agents have conversations.
- **Free up names**, in the header of **Stored without history**, forgets in one go those that never
  received a prompt.

## Agents that sleep

In **Settings → Agents**, **Hibernate idle agents** is off. Turned on, an agent with no activity for
the time set in **Sleep after** is shut down, the panel stays in place with a **Wake up** button, and
the conversation resumes from where it stopped when the agent comes back. Whatever was written in
that terminal until then is lost.

- **Sleep after** ranges from 5 minutes to 8 hours, and comes at 1 hour. The clock resets with each
  tool the agent uses, each prompt you send and whenever you open its panel.
- **Never sleep**: whoever is working, whoever is waiting for an answer from you, and the selected
  panel in the canvas you are looking at.
- **Sending a prompt wakes the agent** and delivers the message, without going through the button.

## When the API knocks an agent down

An agent cut off mid-answer goes into the crashed state, not the ready one. You are notified
according to your [alerts and sounds](avisos-e-sons).

With **Resume agents the API knocks down** on, which is the default, the app tells the agent to carry
on from where it stopped, explaining what happened. The following attempts wait 3 seconds, 30
seconds, 1 minute, 2 minutes and 5 minutes, and stop growing there. After four crashes in a row the
app stops insisting and waits for the provider to come back. Resuming on its own does not suppress
the alert. The switch is in [agent settings](ajustes-agentes), and resuming by hand is in
[talking to them](falar-com-eles).
