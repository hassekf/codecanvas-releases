---
slug: ajustes-aparencia
titulo: Project appearance
resumo: The tab where this project's theme, veil, wallpaper and font are chosen, and where the app's language lives.
area: projeto
nivel: basico
---

In **Edit "project name"… → Appearance**. The sheet opens from the project picker in the bottom bar
and, on the start screen, from the "⋯" on the project card or by right-clicking it.

This is the only tab whose contents belong to the **project**, not to the app. What each choice does
on screen is in [the project's appearance](aparencia).

## The tab's controls

- **Theme**: the ten cards, each with a preview of the background, a glass panel on top and the three
  agent state indicators. Clicking applies it right away. Each card's three buttons choose between
  the animated scenery, the still scenery and colors only.
- **Veil darkness**: how much the background is toned down under the panels, from 0% to 100%. It only
  appears when there is a background, so it does not appear in the "Só cor" style with no wallpaper.
  The **Default** button next to the number appears when the value is off the current theme's
  default.
- **Customize wallpaper**: a collapsed card, which starts open when this project already has a
  wallpaper. This is where you pick a file of your own, or ask for a background by describing what
  you want. The request only appears with the OpenAI key saved.
- **Interface font**: each option written in its own font, with a sample below.
- **Selected panel**: the outline that marks which panel you are in. This is the only item in the tab
  that **applies to every project**.

## The selected panel

- **The color**: the theme's, six suggestions, or any other through the system color picker.
- **Espessura** (thickness): from 0.5 to 4 points.
- **Brilho** (glow): from 0% to 200%. At 0% the outline has no glow.
- **Back to the theme's**: appears at the top of the card when any of the three is off the default,
  and restores all three at once.

The sample just above the controls shows the result as you drag. See
[panels and the desk](os-paineis-e-a-mesa).

## Nothing is written until you save

The screen changes as you choose, but only what you **Save** takes effect. Cancelling or closing the
sheet restores what was there.

This project's theme, background and font are **not erased** by "Restore defaults" in the app's
Settings, which touches only the general preferences.

## The app's language

The language belongs to the whole app, so it is not here. It lives in two places that change the same
thing: the flag capsule in the start screen footer, and the footer of the Settings sidebar.

- There are four options: **System** (the default), **Português**, **English** and **Español**.
  "System" follows the macOS language.
- The picker always shows the flag and the name of the language **in effect**, including when the
  choice is "System".
- The switch is immediate, with no app restart, and no agent is interrupted.
- Dates and numbers follow the chosen language, and so does [dictation](ditado).
- Voice commands and what the assistant says out loud stay in Portuguese.

## The neighboring tabs

The project folder and name in [project settings](ajustes-projeto), the account agents are born into
in [agent settings](ajustes-agentes), the browser home page in [browser settings](ajustes-navegador).
