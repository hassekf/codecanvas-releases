---
slug: quando-algo-nao-funciona
titulo: When something doesn't work
resumo: Symptom and action: what to do about each common CanvasCode failure, and where the app already shows the cause.
area: conta
nivel: basico
---

## The agent panel opens no terminal

The panel says which case it is.

- **"Claude Code isn't installed."**: click **Install now**. The installation is local and asks for
  no administrator password. See [your first agent](primeiro-agente).
- **Another CLI declared as not installed**: the panel shows its installation command. Run the
  command in a terminal and reopen the app. See [multiple providers](varios-provedores).
- **"Preparing the agent…"**: the app is asking the shell where the CLI lives. Wait a few seconds.

## An agent stopped mid-task and looks like it finished

That is the provider dropping the agent. The app alerts you with a notification that does not go
away on its own and, with automatic recovery on, tells the agent to continue, spacing out each new
attempt. It does not insist against a rejected credential, a service that is down, or a conversation
that is too full.

- **To turn recovery on or off**: **Resume agents the API knocks down**, in
  [agent settings](ajustes-agentes). When off, the crash is still shown and announced, and you
  resume through the alert's button, by voice, or by typing in the agent's terminal.
- **To find out whether this is happening too often**: **Settings → Diagnostics**, under **Crashes
  from API errors**. It covers the last seven days, per provider, with how many were resumed
  automatically and a chart by day. **Clear log** resets the count.

## I don't know whether the problem is mine or the provider's

In the footer, each provider's badge shows the state of its service. Hover to read the message, and
click to open the status page in a browser panel.

## An agent came back remembering nothing

An agent's conversation lives inside the account it was born in. The app tells you which account it
looked in and, when the conversation is in another registered account, which one it is.

**Switch that agent's account** to bring the conversation over: right-click its panel and pick from
the account menu. The app does not move the conversation on its own. See
[accounts and profiles](contas-e-perfis).

## An agent says it has no permission to read a file

macOS asks CanvasCode for permission to reach Documents, Desktop and Downloads, and the agent gets
nothing but an access-denied error.

Grant it in **System Settings → Privacy & Security → Files and Folders**. See
[the permissions macOS asks for](permissoes-do-mac).

## Nina can't hear you

1. Open **Settings → Diagnostics** and read the **Microphone** state. It is written in Portuguese:
   `liberado` (granted), `negado` (denied), `bloqueado` (restricted) or `nunca perguntado` (never
   asked).
2. On `nunca perguntado`, click **Ask for permission**.
3. On `negado` or `bloqueado`, click **Delete the permissions and ask again**. macOS does not ask
   twice, and this button deletes this app's permission record so it starts asking from scratch. The
   app reopens right after, and nothing else is deleted.
4. When it is `liberado`, check the **Microphone** in **Settings → Voice** and use **Test the
   microphone**, just below it. A meter stuck at zero is usually macOS capturing from another
   device.

If she stops hearing you in the middle of a conversation that was working, the voice indicator shows
"reconnecting…" and the connection comes back on its own. More in
[setting up voice](configurar-a-voz).

## The Issues and PRs tabs are empty

They depend on `gh`, GitHub's command line tool. The tab itself says which case it is: `gh` not
installed, `gh` not logged in (`gh auth login`), or the project with no GitHub remote. See
[the Git panel](painel-git).

## The app won't open

After crashing twice in a row at launch, the app comes up on a recovery screen, without loading the
projects or the agents, offering the backups.

Pick a point in the list and click **Restore everything**, **Settings only** (when it was a
preference that broke the app) or **Projects only**. The current state is saved before restoring.
With no backup in the list, all that is left is to open anyway, and the app tries to start from
scratch.

The same screen is in **Settings → Backups**, under **Restore from a backup…**, next to **Back up
now** and the copy frequency.

## Something got strange after I changed settings

**Restore defaults**, at the bottom of the Settings sidebar. It asks for confirmation and returns
the font, the scale, the maximum width, the shortcuts, the voice and the subagent panels to their
originals, and unpins the Claude Code version. Not affected: your OpenAI key, the audio devices and
the canvas themes.

## The installer shows up as damaged

The download came in incomplete. Download it again. See [installing](instalar).

## Reporting a problem

- **The version number** is at the bottom of the Settings sidebar.
- **The voice log** records every connection, drop and reconnection. The **Show in Finder** and
  **Open** buttons are in **Settings → Diagnostics**, and it always records.
- **The macOS crash reports** can be sent through the **Send crash and failed-resume reports**
  switch, in the same place. The list of recorded crashes sits just below, with a **Send** button on
  each. See [where my data lives](onde-ficam-meus-dados).
