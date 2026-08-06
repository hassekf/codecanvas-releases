---
slug: contas-e-perfis
titulo: Accounts and profiles
resumo: Where agent program installations are registered, which one each project and each agent is born on, and what happens to the conversation when you switch.
area: agentes
nivel: basico
---

An account is a configuration folder of the agent program. The login, the settings and the agents'
conversations live inside it, which is why the account decides what memory an agent has available.

## The list of accounts

In **Settings → Agents → Claude installations**.

- **The default installation**: the folder your terminal already uses. It is always on the list and
  cannot be unregistered.
- **Rename**: changes an account's name. That name appears in the header of every agent born on it,
  and only when more than one account is registered. An empty name restores the original label.
- **Add installation…**: opens the folder picker, with hidden items shown, and registers the chosen
  folder. Nothing is copied: the app simply points to it. The suggested name comes from the folder
  containing the chosen one when its name starts with a dot. The same folder is never added twice.
- **Remove from the list**: unregisters the account. If any agent is born on it, the app asks first
  and offers **Bring the conversations over to the default one** or **Remove and leave the
  conversations there**. Nothing is deleted from disk in either case, and the conversations come back
  if you register the folder again.

Each row shows the folder path and its state: a folder never used warns that the first agent will ask
for the login, and a folder that left the disk is flagged as missing.

An account's agent program is inferred from the folder's contents, not chosen by you. An account belongs
to a single program. See [several agent programs](varios-provedores).

## The project's account

In **Edit the project → Agents → Claude installation**. With a single account registered, the menu
shows the default one and the instruction to register the others in Settings.

- **The choice applies to the whole canvas**: every agent born there uses that account, except the
  ones that picked an account of their own.
- **When you save a switch with agents open**, the app asks between **Bring the conversations over**
  and **Start fresh on the new account**, and the agents that inherit the project's account are
  reborn on it. The conversation comes back whole; the turn in progress at that instant is lost.
  Agents that picked their own account are untouched.
- **If the chosen folder no longer exists**, the screen warns you right there: the agent will be born
  logged out.

## An agent's account

In the agent panel's menu, under **‹name›'s account**. The item only appears when another account of
the same agent program is registered.

- **The options** are the project's account, the default installation and each registered account.
  The current one is checked and cannot be picked again.
- **Picking one changes nothing right away**: it opens a question. If the agent has already talked,
  the question offers **Bring the conversation over** or **Start fresh there**; if it never talked,
  only **Change**.
- **Bring the conversation over** copies its past into the new account's folder, and it comes back
  remembering everything. Starting fresh keeps the two accounts separate on disk. The old
  conversation is not deleted in either case.
- **The choice belongs to that agent**: switching the project's account later does not drag it along.
- **The agent is reborn on the new account**, with the same name and the same place on the canvas.
  Whatever it was doing at that instant is lost.

## When an agent comes back without the conversation

The conversation lives inside the account's folder. Calling an agent back on an account other than
the one it worked on brings it back with the right name and a blank memory.

The app warns you in that case and says which account it looked in. If the conversation is on another
registered account of the same program, it says which one, and does not fetch it: fetching it is the
account switch described above.

## Configured elsewhere

- The agent programs available: [several agent programs](varios-provedores).
- How the agents of this canvas are born: [project settings](ajustes-projeto).
- Calling a stored agent back: [creating and closing agents](criar-e-fechar).
