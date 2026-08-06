---
slug: painel-custos-e-desempenho
titulo: Usage and performance
resumo: Two panels: how much of each provider's subscription is gone and what each agent cost, and how much memory and CPU the app is using, per process.
area: paineis
nivel: basico
---

The usage panel opens with `⌘K` (type "uso", "consumo" or "limite"); the performance one, with
"desempenho", "cpu" or "memória".

## The usage panel

One block per provider with a known limit. In each block:

- **The limit windows** of the subscription, each with the percentage already spent and when it
  resets. The larger ring repeats the tightest window, which is the one that stops the work first.
- **The plan**, when the provider reports it.
- **The credits**, when they exist: how much was used and the ceiling, in the account's currency.
  They keep working after a window runs out.
- **seen**: when that number was last read. Providers that only publish usage when a session runs
  may be showing a number from days ago.

Below the blocks, a dimmed line with a **dash** lists the providers whose usage cannot be read:
Gemini, Cursor and Grok. The dash means "unknown", not zero.

### In this canvas

Under **ON THIS CANVAS**: the total spent by this canvas's agents, and one row per agent with the
name you gave it. Each bar is proportional to the largest spend in the canvas, not to an absolute
value.

The value is an **estimate**: the price does not come from the conversation, it comes from a built-in
price table.

### Separate accounts count separately

A limit belongs to the account, not to the project. With more than one account of the same provider
in use, each gets its own block, labeled with the account name. What one canvas consumes counts
against the same account in every other one. See [accounts and profiles](contas-e-perfis).

### The footer capsules

One capsule per provider in use, with two clickable halves:

- **The provider logo**: changes appearance depending on whether the service is up or having an
  incident. Clicking opens that provider's status page in a browser panel in here.
- **The ring with the percentage**: the tightest window of that account. Clicking opens the usage
  panel.

With more than one account on show, the initial of the account name appears before the ring.

What the assistant and the voice spend is a separate bill, and it is in
[what it costs](quanto-custa).

## The performance panel

It measures the app, the agents, the servers the agents start, and the browsers, even with the panel
closed.

- **MEMÓRIA** and **CPU DA MÁQUINA**: the two current numbers, with a graph of the preceding
  minutes.
- **The line below the numbers** compares against the norm: either **no normal deste app**, or how
  many times the norm the app is weighing right now. It is the deviation, not the number, that
  triggers a report.
- **WHERE THE MEMORY IS**: the split by role, across **O app**, **Agentes**, **Servidores dos
  agentes**, **Browsers** and **Terminais**.
- **WHO'S PULLING**: the six heaviest processes, with the name of the panel each one belongs to.
- **Save report**: writes a report of everything happening right now and opens it in a panel.

When the system does not allow identifying which WebKit processes belong to the app, the panel warns
that the browsers are **not** being counted.

### The number in the bar

Next to the zoom sits the memory in use, plus the CPU percentage when it goes above 10%. It gains
color as it approaches your spike threshold. Clicking opens the performance panel. It disappears
when the monitor is off.

### What counts as a spike

In **Settings → Performance**.

- **Measure and save peak reports**: turns the monitor on. Off, nothing is measured, no report is
  saved, the panel shows a button to turn it back on, and the number leaves the bar.
- **Sensibilidade**: from +10% to +200% above what the app usually weighs. The screen translates the
  percentage into today's number ("aviso acima de X"), and the norm is learned in about a minute of
  the app being open.
- **Open the folder** and **See the last one**: the reports folder, and the most recent report in a
  panel.

Each spike becomes a file with the processes, the agents, what was open, and the preceding minutes.
The 30 most recent are kept, and none of them leaves your machine.
