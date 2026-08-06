---
slug: ajustes-agentes
titulo: Agent settings
resumo: The Agents tab, control by control, and the three agent settings that live in the Interface tab.
area: ajustes
nivel: basico
---

In **Settings → Agents**. What is here applies to every project. What belongs to a single project
(the account its agents are born in, the model, the permissions, the default browser) lives in the
canvas settings. See [project settings](ajustes-projeto).

- **The agent's delivery history**: on, each completed subject becomes a line on the back of the
  panel when the agent moves to the next subject. Off, the back shows only what it is doing now.
- **Resume agents the API knocks down**: on, the app tells the agent to carry on from where it
  stopped after an API crash, waiting longer with each new attempt. The crash alert happens whether
  it is on or off. See [creating and closing](criar-e-fechar).
- **Hibernate idle agents**: off by default. On, an agent with no activity for the time below is shut
  down, the panel keeps a wake button and the conversation resumes when the agent comes back.
  - **Sleep after**: appears inside the control above, and only with it on. It ranges from 5 minutes
    to 8 hours, and comes at 1 hour. The clock resets with each tool used, each prompt sent and
    whenever you open the agent's panel. Never sleep whoever is working, whoever is waiting for your
    answer and the selected panel in the canvas in focus.
- **Claude installations**: registers `.claude` folders, each with its own login, servers and
  conversations. **Add installation…** asks for the folder. Removing one from the list deletes
  nothing from disk, and the app asks what to do with the agents that depended on it. See
  [accounts and profiles](contas-e-perfis).
- **Claude Code version**: **The latest** keeps Claude Code updated on its own when the app opens,
  before any agent is born. The menu also lists the versions present on the machine, and pinning one
  turns off automatic updating. The change applies to agents created from then on.
- **Pull request badge**: shows each agent's PR on the panel, in the footer and in Git, with the
  state of continuous integration. Off, the app stops asking GitHub about your PRs. See
  [the Git panel](painel-git).
- **Dev servers in their own panel**: off by default. On, long commands such as a dev server or a
  file watcher are opened in a visible terminal panel, instead of running inside the agent. See
  [talking to them](falar-com-eles).
- **Isolation by worktree**: on, each agent creates its own copy of the project before writing and
  commits on its own branch. The text of the protocol the agents receive is editable right below, and
  the editor only appears with the switch on. See [worktrees and isolation](worktrees-e-isolamento).
- **Subagent panels**: **Show subagents on the canvas** gives a panel to each task an agent delegates,
  up to three at a time. Off, subagents keep working without showing up. See
  [one agent calls another](um-agente-chama-outro).
- **Conversations between projects**: how many messages one authorization of yours allows between an
  agent here and an agent in another project. The options are 2, 4, 6, 10 and 20 messages, and the
  default is 4. Once used up, they need a new authorization.

## In the Interface tab

- **Glow on the panel when done**: the panel border glows when the agent delivers, even without being
  selected.
- **Highlight the area tab when done**: the area tab flashes when an agent finishes, or starts
  waiting for you, in an area you are not looking at.
- **Completion glow color**: the color of the two above. The **Default** button only appears after
  you change it, and puts it back.
- **Group the agents into tabs**, in the **Workstreams sidebar** section: in an area with more than
  one agent, they share a single panel, with the chosen one on show and the others in tabs. It
  applies to areas never configured by hand; each area's context menu overrides it. See
  [work areas](areas-de-trabalho).
- **Hide the area tabs while it's docked**, in the same section: the tabs at the top disappear and the
  workstreams sidebar takes over listing the areas, switching on click, creating, renaming and
  flashing. The control only works with the sidebar docked.
