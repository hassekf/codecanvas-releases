---
slug: painel-midia
titulo: The media panel
resumo: YouTube and YouTube Music in the canvas: the two modes, cinema mode, the two ways to minimize and the silence when voice takes over.
area: paineis
nivel: basico
---

Open it with `⌘K` and `mídia`, `vídeo` or `música`. There is a single panel in the whole app: asking
for media in a canvas where it isn't brings the panel here, instead of opening a second one.

## The two modes

The selector in the bar switches between **Vídeo** (YouTube) and **Música** (YouTube Music). It is
the same account in both.

- **Each mode keeps its own place**: you go to music and come back to video at the point where you
  were.
- **One plays at a time**: the mode that leaves the screen is paused, not reloaded.
- **Closing the panel stops everything.**

## The bar

- **Só o vídeo** (video only): hides the page and lets the video fill the panel. Clicking again
  brings the site back, with search and recommendations, at the same point in the video. Available in
  Vídeo mode only.
- **Back**: goes back one page. Unavailable when there is nowhere to go back to.
- **Início** (home): loads the home page of the current mode.
- **Reload**: reloads the page, and becomes a stop button while it loads.
- **Minimizar como papel de parede** (minimize as wallpaper): appears in Vídeo mode only. See below.
- **Minimizar** (minimize): shrinks the panel into a capsule beside the command bar, and the sound
  keeps playing.

## The wallpaper

**Minimizar como papel de parede** sends the video to the back of the canvas: it fills the screen and
plays behind the panels.

- **Clicks pass through**: to touch the video, bring it back from the capsule.
- **Restoring the panel ends the mode**, and the canvas background returns to what it was. See
  [appearance](aparencia).
- **The wallpaper is never paused by voice**, not even during a conversation with Nina: its volume is
  lowered and it keeps running.

## When the media goes quiet

Five things ask for the audio, and the media gives back what was playing when the last of them is
done.

- **A conversation with Nina**: pauses the media before the microphone opens, and resumes at the
  point where it stopped.
- **Dictation, command mode, an alert and reading aloud**: lower the volume and leave the video
  running.

If you were the one who paused during the conversation, the app does not start it again: it only
resumes what it silenced itself. See [talking to Nina](falar-com-a-nina).

## The Google account

This panel's sign-in is kept apart from the rest of the app, and the agents do not reach it through
the canvas browsers.

- **The Google sign-in window** opens inside the panel's own page.
- **When Google refuses the sign-in** because this is an embedded browser, the panel says so and
  offers **Continue without signing in**. With no account, you can still search and watch, without
  history or playlists.

## Who else puts things on

Nina, by voice: play, pause, switch mode, open an address, search a term, enter and leave cinema
mode, minimize and restore. The panel is born if it doesn't exist yet.

An agent can put something on too: it passes the address it chose, and the video starts playing on
your screen. The mode is decided by the address. It can instead send a search term and leave the
list of results on screen for you to choose. See [the agent works the canvas](o-agente-mexe-no-canvas).

In **Settings → Tools**, turning off the **Mídia** group removes voice control and changes nothing in
the panel.
