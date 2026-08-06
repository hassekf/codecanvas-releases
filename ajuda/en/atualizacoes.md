---
slug: atualizacoes
titulo: Updates
resumo: The automatic check, the button to check now, what happens to the agents at install time, and each version's release notes.
area: conta
nivel: basico
---

The app looks for a new version on its own, in the background, every hour, and at launch when that
interval has already passed since the last check.

## Asking now

Two doors, and both do the same thing:

- **The app menu → Check for Updates…**
- **Check for Updates**, in the footer of Settings, next to the version number. It closes Settings
  before checking, and is unavailable while a check is under way.

The check you ask for answers even when there is nothing new. The automatic one is silent.

## The agents that are working

- **The automatic check does not offer an update while an agent is working.** It does not insist and
  downloads nothing: the next check looks again and offers the newest version at that point.
- **The check you ask for goes ahead anyway.** If you tell it to install while someone is working, the
  app lists by name who is about to be shut down and offers **Adiar** (postpone) or **Instalar mesmo
  assim** (install anyway).
- **Postponing leaves the update downloaded and waiting.** Until it is installed, that is the version
  offered again, and newer ones do not show up.
- Each agent's session is saved and you can call them back by name. Whatever they are doing at the
  moment of the install is lost.

## What's new

- **What's New**, in the footer of the start screen: opens what changed, version by version, with
  yours marked.
- **The dot next to the button**: lights up when there is a version you haven't read yet, and goes
  out when you open the list.

The list is written for whoever uses the app. The technical part of each version is left out of it.

## Why you can trust what it downloads

Every update is signed, and the app refuses any file whose signature does not match the key it
carries. On top of that, the downloaded binary still goes through Apple's check, which is what makes
the app open with no unidentified developer warning. See [installing](instalar).

## When it doesn't update

In the order it usually happens:

1. **No internet, or a network that blocks access.** Ask through the button to see the answer.
2. **There is always someone working.** Use the button and install when you can shut the agents down.
3. **A postponed update, waiting.** Install it, and the next ones start arriving again.
4. **None of the above.** Download the app again and install it over the old one. Canvases,
   conversations and settings do not live inside the app: see [where my data lives](onde-ficam-meus-dados).
