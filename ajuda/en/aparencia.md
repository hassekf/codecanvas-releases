---
slug: aparencia
titulo: The project's appearance
resumo: Theme, background scenery, veil, wallpaper and interface font, chosen per project.
area: canvas
nivel: basico
---

Everything on this page is chosen in the **Appearance** tab of the project sheet: open the project
picker in the bottom bar and click **Edit "project name"…**. On the start screen, the same place is
reached through the "⋯" on the project card or by right-clicking it. The tour of the controls is in
[project appearance](ajustes-aparencia).

The choice belongs to each project. Changing it here touches no other project.

## The themes

There are ten, one card each: Meia-noite (the default), Grafite, Forja, Bosque, Ameixa, Enseada,
Rubi, Aurora, Terracota and Marfim. Their names are in Portuguese in every language. The card preview
shows that theme's background, a glass panel on top and the three agent state indicators.

Clicking a card applies the theme on screen right away. Nothing is written until you save the sheet,
and closing without saving restores what was there.

**Marfim** is the only light one: it turns the whole interface to the light side. Two consequences:

- **The rectangle where the agent writes stays dark.**
- **The start screen stays dark**, as it comes before any project.

## The theme's scenery

Each theme brings its own scenery, which ships inside the app and is not downloaded. The card's three
buttons decide what to do with it:

- **Animado** (animated): the scenery video, looping and muted. This is the default. It is
  unavailable on a theme with no video.
- **Parado** (still): the frozen scenery. When the theme offers more than one scene, the thumbnails
  appear inside its card so you can pick which one.
- **Só cor** (color only): no scenery, just the theme's gradient.

Clicking one of these buttons on another theme's card switches the theme and the style at once. The
chosen style applies to every theme; the chosen scene applies only to the theme in use.

The video pauses on its own when the window is hidden behind another app or minimized.

## The veil

The **Veil darkness** control decides how much the background is toned down so the panel text
survives on top of it. It applies to the theme's scenery and to your wallpaper, and goes from 0% to
100%; at 0% the background shows as it is.

- It **disappears from the screen** when there is no background at all, that is, in the "Só cor"
  style with no wallpaper.
- The **Default** button appears next to the number when the value is off the current theme's
  default.
- Switching between a dark theme and Marfim **moves the veil along**, and only while it is still at
  the default of the side you are leaving. Once you have touched it, no theme change moves it.

## The wallpaper

In the **Customize wallpaper** block you put a file of your own in place of the scenery. It starts
collapsed, unless this project already has a wallpaper.

- **Choose file…** accepts images, GIFs and video (MP4, MOV and M4V). Video and GIF loop, muted. The
  file is **copied into the app's folder**, so deleting the original later does not delete the
  background.
- **Change** replaces it, **Remove** brings the theme's scenery back.
- While your file is there, it wins over the theme's scenery, and the Animado, Parado and Só cor
  buttons stop changing what you see. The rest of the theme still applies.

### Asking for a background instead of picking a file

The **Or ask for one** block, inside the same card, only appears with the OpenAI key saved in
[setting up voice](configurar-a-voz). You describe the background and choose between two buttons:

- **Search**: looks on the web for an image that already exists and returns a grid of candidates to
  click. It is fast, and it is the way to something specific and real.
- **Create**: paints an image from the description. It takes about 40 seconds, costs a few cents of a
  dollar, and comes one at a time.

## The interface font

The **Interface font** menu shows each option written in its own font, with a sample below. It
applies to the whole app while this project is open.

The **terminal** font is a different one, belongs to the whole app, and lives in
**Settings → Terminal**, next to its size.

## The panel glass

Two controls in **Settings → Interface** decide how much of the canvas shows through behind the panel
text. They apply to the whole app, not to one project.

- **Panel glass blur**: how much the background behind the panel disappears. The control moves in steps.
- **Panel opacity**: the layer on top of the glass, from 0% to 100%. Raising the opacity hides the
  effect of the blur.

## By voice

With the assistant set up:

- *"switch the theme to forja"*: it knows all ten by name.
- *"put a forest background with fog"*: it **paints** by default. Saying "search", "find it online"
  or asking for something specific and real makes it search the web.
- *"find another one"*: swaps in the next candidate without you repeating the description. It is
  instant while there are candidates saved.
- *"remove the background"*: drops the wallpaper and brings back the theme's scenery.

The first three need the OpenAI key.

Asking for an **image** is a different thing: it is pasted onto the canvas and kept in the gallery.
See [the gallery panel](painel-galeria).
