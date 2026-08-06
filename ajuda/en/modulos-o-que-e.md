---
slug: modulos-o-que-e
titulo: What a module is
resumo: A panel written by you, which lives on the canvas like the native ones and talks to the app.
area: modulos
nivel: avancado
---

A module is **a panel of your own**. You (or an agent of yours) write a page, and it starts living on
the canvas like any native panel: it opens from `⌘K`, joins the layout, minimizes into the shelf and
can be opened by voice.

It's for whatever only makes sense to you: the balance of an account, the dashboard of a machine you
administer, a counter done your way, the screen of an internal system nobody else uses.

## Where it lives

In a folder inside the app's folder, one per module. Two pieces are required: the manifest, which
declares what the module is, and the starting page.

**There is no installer and no registry.** The app watches the folder: creating makes the module
appear, fixing brings it back, deleting takes it out of the app. While you are writing, saving a file
reloads that module's panels without restarting anything.

**The module belongs to your machine, not to the project.** It is available in every canvas, and each
opening creates a panel of that canvas: the page knows which project it is in, and the same module can
show different things in each one.

## What it gains by being inside the canvas

An ordinary page in a browser can do none of this:

- **Make a request with no origin restriction**, because the one fetching is the app.
- **Run a script from its own folder**, with the output coming back to the page.
- **Know which project it is in**, and adopt that canvas's theme and font.
- **Store data** between openings and across canvases.
- **Alert you** inside the app, with sound, reading aloud and a button that takes you to the panel.
- **Give tools to Nina and to the agents**, so they can use the module by speaking.

The detail of each one is in [a module's capabilities](modulos-capacidades).

## What it is not

- **It is not an extension of the app.** It draws inside its own panel and doesn't change the rest of
  the interface.
- **It is not distributable.** There is no store, no registry and no installing by link: the folder is
  yours.
- **It doesn't run without you.** A module that needs a secret keeps the secret in a script in the
  folder, and not in the HTML.

## Where to go next

- Creating one: [creating a module](modulos).
- The panel on screen and the list of modules: [a module's panel](painel-modulos).
