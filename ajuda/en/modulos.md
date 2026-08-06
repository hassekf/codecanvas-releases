---
slug: modulos
titulo: Creating a module
resumo: The folder, the manifest, the actions that become voice tools, and what the page can do through the app's bridge.
area: modulos
nivel: avancado
---

A module is a folder in `Application Support/codeCanvas/modulos/<id>/`, and the folder name is the
module id. Two pieces are required: `modulo.json` and `index.html`. How it behaves once it's done is
in [a module's panel](painel-modulos).

There is no installer and no registry: the app watches the folder. Creating makes the module appear,
fixing brings it back, deleting takes it out of the app.

## Asking an agent

Ask an agent on the canvas: *"create a module that shows the balance of my account at bank X"*. It
stamps out the folder from the skeleton, edits it, opens the panel, takes a picture of it, reads the
console and fixes what's wrong.

The skeleton comes with the manifest filled in, a page that already uses the bridge, an example
script already declared as an action, and a `CONTRATO.md` file with the full reference for this
version of the app.

The id comes from the name, lowercased, without accents or spaces. A name that collides with a native
panel of the app is refused, and so is an id that already exists.

## The manifest

- **`formato`**: the contract version. Required, and today it is `1`. A version newer than the app
  knows is refused whole, with the reason.
- **`nome`**: required. It's the name in the panel, in `⌘K` and in voice.
- **`descricao`**: the line under the name in the catalog and in the panel bar.
- **`icone`**: an SF Symbols name.
- **`palavras`**: synonyms the `⌘K` search accepts.
- **`varios`**: `true` allows more than one panel of this module per canvas.
- **`usaContexto`**: documents that the content varies per project. It doesn't change the app's
  behavior.
- **`recarregarACada`**: reloads the page on its own every N seconds, 5 minimum.
- **`semMoldura`**: `true` makes the loose panel hide its header and border.
- **`acoes`**: the tools the module gives Nina and the agents.

## The actions

Each action has a **`nome`** (lowercase, digits and `_`), a **`descricao`** and a **`script`** from
its own folder. When called, the app runs the script and returns the standard output to whoever
called it; Nina answers by speaking on top of it.

The `descricao` is the field that decides when the action gets called: write what it does, what it
returns, and on which request to use it. Vague, it gets called at the wrong time, or never.

The output has to be short and readable. Errors go to the error output, with a non-zero exit code,
and that is what the app passes on as a failure.

Nina receives the actions when the conversation opens: turning a module's switch on or off applies
from the next conversation. Both switches are in [a module's panel](painel-modulos).

## What the page can do

The page gets a bridge to the app: a request with no origin restriction, running a script from the
folder, knowing which project it is in, adopting the theme, storing data and notifying you. It is in
[what a module can do](modulos-capacidades).

## Where to go next

- The concept: [what a module is](modulos-o-que-e).
- The panel on the screen and the list in Settings: [a module's panel](painel-modulos).
