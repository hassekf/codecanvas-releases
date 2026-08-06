---
slug: permissoes-do-mac
titulo: The permissions macOS asks for
resumo: Each permission the system asks about, what it unlocks, what breaks if you deny it, and how to make the Mac ask again.
area: comecando
nivel: basico
---

macOS asks the first time you use each feature. None of them is requested at launch.

## The permissions

- **Microphone**: without it, voice conversation and dictation don't work. See
  [setting up voice](configurar-a-voz).
- **Speech recognition**: used by the dictation that runs on your own Mac. See
  [dictation](ditado).
- **Screen recording**: without it, recording the app window doesn't work. See
  [the recording panel](painel-gravacao).
- **Camera**: the image appears in [the webcam panel](painel-webcam-e-avatar) and does not leave your
  Mac.
- **Calendar**: the app reads your calendar to warn you about meetings and open the call link.
  Nothing is written to your calendar. See [calendar and meetings](agenda-e-reunioes).
- **Notifications**: macOS alerts while the app is in the background. The request only happens after
  you turn on "Notify on the Mac outside the app" in [alerts and sounds](avisos-e-sons).
- **Desktop, Documents and Downloads**: the folders where the agents read and write.

## Folder access

**macOS charges the permission to CanvasCode, not to the agent program.** An agent opened in here is
a child process, and the system assigns the access to the responsible app.

Denying it does not produce a permission prompt in the agent's terminal. The agent gets a plain
access-denied error, and often concludes that the file doesn't exist.

To allow it later: System Settings → Privacy & Security → Files and Folders, and enable CanvasCode
for the folder in question.

## When macOS stopped asking

A denied permission is not asked about again: the request answers "no" straight away, with no dialog.
This also happens when an old permission record for this app was made by a binary with a different
signature, such as a development build or an earlier version.

In **Settings → Diagnostics** you'll find:

- the state of **Microphone**, **Speech recognition** and **Screen recording**;
- **Ask for permission**, which only has an effect while the system hasn't decided yet;
- **Open System Settings** and **Screen Recording in System Settings**, which lead to each system
  pane;
- **Recheck**, which re-reads the state;
- **Delete the permissions and ask again**, which appears when one of them is denied. It deletes this
  app's permission record and nothing else. **The app has to be reopened afterwards**, and the
  questions start over.
