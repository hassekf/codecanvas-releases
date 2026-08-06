---
slug: ajustes-navegador
titulo: Browser home page
resumo: Which address a new browser opens in this project, and when that choice does not apply.
area: projeto
nivel: basico
---

In **Edit "project name"… → Browser**. The tab has one control: **Home page**.

## The field

- **What it accepts**: the address as a person types it. `github.com` becomes `https://github.com`,
  `localhost:3000` works, and an address already starting with `http://` or `https://` goes through
  as it is.
- **The line below the field** shows which address it will actually open, and changes as you type,
  with no need to save.
- **Blank opens Google.**

The choice belongs to each project, and nothing is written until you save the sheet.

## When it applies

It applies to the browser **you** open, through `⌘K` or the panel catalog, and to the one the voice
assistant opens at your request.

It does **not** apply to the browser an agent opens to show you something: that one already comes
with an address. See [the browser panel](painel-navegador) and
[the agent sees the browser](o-agente-ve-o-navegador).

## The other browser choice

The **Agents** tab of the same project has **Default browser**, with two options:

- **Internal**: the agent shows what it produced in the browser inside the canvas. This is the
  default.
- **External**: the agent opens it in your system browser, and only uses the internal one when you
  ask.

That one answers where the agent shows things; this one answers which page an empty browser opens.
The details are in [agent settings](ajustes-agentes).
