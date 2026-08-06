---
slug: painel-modulos
titulo: A module's panel
resumo: How to open a panel you wrote yourself, what its bar does, and the two switches every module has.
area: modulos
nivel: avancado
---

A module is a panel written by you (or by an agent of yours) and installed in a folder on your Mac.
To write one, see [modules](modulos).

Open it with `⌘K` and the module's name, or the search words its manifest declared. By voice, the
module is opened by the name in the manifest.

By default it is one panel per canvas: asking for the same module again selects the panel that
already exists. A module can declare that it accepts several.

The module is available in every project. Each
opening creates a panel of that canvas, and the page knows which project it is in: the same module
can show different things in each one.

## The panel bar

- **The line on the left**: the description from the manifest.
- **Reload the module**: reloads the page.
- **Reveal the folder in Finder**: opens the module's folder.

A module can declare that it lives outside the grid. In that case the header, the border and this bar
disappear while the panel is loose, and the content fills the whole panel; a click reveals the
controls again, and putting it back in the grid brings the frame back.

A module can also declare a reload interval (5 seconds minimum), and then the page reloads on its
own.

## While you write the module

The app watches the folder: saving a file reloads that module's panels, without restarting anything
and without reopening the panel. Panels of other modules are left alone.

The panel also speaks up when something is wrong, instead of going blank:

- **This module has a problem**: the manifest or the folder didn't pass validation. The text says
  what, and the button reveals the folder in Finder.
- **This module no longer exists**: the folder is gone from disk. If it comes back, the panel comes
  back with it.
- **This module is turned off**: the module is intact, but switched off in Settings.

A JavaScript error on the page doesn't bring the app down: it stays in that page's console, and the
agents read that console.

## Settings → Modules

The screen lists the valid modules and the ones that failed validation, the latter with the reason
written out and a **Reveal** button.

- **Each module's switch**: when off, the module disappears from search, from voice and from the
  agents' reach. A panel of it that is open says the module is turned off, instead of vanishing in
  front of you.
- **Tools for Nina**: only appears on a module that is active and has actions. When off, the assistant
  goes back to only opening and closing the panel, and the actions leave her vocabulary on the next
  conversation.
- **Reveal the modules folder in Finder**, at the bottom: opens the folder where all of them live.

A new module is born active and with its actions available.
