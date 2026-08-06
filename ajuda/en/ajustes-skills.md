---
slug: ajustes-skills
titulo: Settings · Skills
resumo: The screen that lists the skills this project has at hand, turns each one on and off here, and installs from the public registry.
area: projeto
nivel: avancado
---

In **Edit the project → Skills**. The tab only exists on a project already created.

## The list

Skills come grouped by origin, and each row brings the name, the description and one tag per agent
program that sees it.

- **In this project**: they are in the repository and versioned with the code.
- **Provider-wide**: they are in your account and apply to all your projects.
- **From the system**: native to the agent program. They carry a padlock, open read-only and cannot
  be removed.
- **With no agent program installed on the machine**, the tab says so and lists nothing: there is
  nowhere to discover skills from.

## Each row's switch

- **Turning it off** asks the agents of this project not to use that skill, and applies to agents
  started from then on. Whoever is already running stays as it was born.
- **The disabled skill stays on the list**, dimmed, and nothing leaves the disk.
- **The effect is limited to this canvas.** The same skill keeps applying in your other projects.

## Each row's menu

- **View / edit SKILL.md**: opens the skill file for reading and editing. On system skills, reading
  only.
- **Remove…**: deletes the skill from disk, including the shortcuts that shared it between agent
  programs. It asks for confirmation and has no undo. To stop using it here only, use the switch.

## Installing

**Install skills…**, at the top of the tab, opens the search in the public registry.

- **The search field** filters by subject, technology or name, and each result brings a description,
  stars and the source repository.
- **Picking a result** opens the confirmation, with the link to the repository. It is third-party
  code, and the source is checked right there.
- **Where to install**: **In this project**, versioned in the repository, or **In my account**,
  applying to all your projects.
- **With the registry down**, the window says so instead of going on searching.
- **The installation fails** when the repository is private, down, or has no skill file at the given
  path. The reason appears in the window itself.

## Configured elsewhere

- What a skill is, and what you can ask an agent: [skills and MCP servers](skills-e-mcp).
- This project's tool servers: [Settings · MCP](ajustes-mcp).
