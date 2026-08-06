---
slug: um-agente-chama-outro
titulo: One agent calls another
resumo: Delegating by voice, agents that bring colleagues onto the canvas, the subagent panels and conversations across projects.
area: agentes
nivel: basico
---

## You delegate

- **Delegating by voice**: hands the task to an agent of this project. With no agent free, the app
  creates one. Saying a name sends the task to that agent, including one that is stored away, which
  comes back on its own to receive it.
- **Calling one back**: brings a stored agent back with the whole conversation. See
  [creating and closing agents](criar-e-fechar).
- **An ambiguous name is never guessed**: when two names come out equally likely, the app asks which
  one before sending anything.

## An agent brings colleagues

An agent at work can open other agents on the canvas, with a task for each one. They are born with
their own panel, terminal and name, and each one can be from a different agent program.

- **Opening without a task** leaves the agent empty, and no prompt is sent to it.
- **Whoever opened them gets the result** from each one when it finishes, including when the task
  goes wrong.
- **Whoever opened them is woken once**, when every agent of that request has answered.
- **Whoever opened them can dismiss** the agents it brought. The panel disappears and the memory
  stays stored.
- **Nobody commands an agent they did not bring.** An agent can read what another one received, what
  it has done and what it said last, but only talks to whoever brought it or to whoever it brought.

## The subagent panels

When an agent splits its own work, each split gets an activity panel with the task it received, the
tools in use and the final answer. The panel stays after it is done, and it is not a terminal.

- **Show subagents on the canvas**, in **Settings → Agents**: turns those panels on and off. When
  off, the subagents work all the same and the app closes the panels that were open.
- **The subagents button on the command bar**: the same switch, with its state in sight.
- **The ceiling is three panels per canvas at a time**, even with the switch on. One agent can fire
  off dozens of subagents, and the ones past the ceiling work without a panel.
- **Each panel is born in the work area of the agent that launched it.**

## Agents from different projects

No conversation across projects starts on its own.

- **The agent asks for permission**: the question appears on your screen with who wants to talk to
  whom, the other one's project, the reason and the message allowance. **Let them talk** opens the
  line; **No** refuses. The message it had held back goes out the moment you authorize.
- **You open a conversation by voice**, saying who talks to whom and about what.
- **What you authorize is the conversation**, not each message: one yes covers that pair of agents,
  that subject and an allowance of messages counting both sides.
- **The allowance does not renew with time.** When it runs out the conversation stops, and the agent
  has to ask for more rounds saying what is still missing. That request arrives as a new question on
  your screen, with **Let them continue** and **End it**.
- **Conversations between projects**, in **Settings → Agents**: sets the allowance of each
  authorization. The options are 2, 4, 6, 10 and 20 messages, and the default is 4.
- **The panel header** shows who the agent is talking to, from which project, and how much of the
  allowance is already spent. Clicking that badge takes you to the other agent's panel.
- **Product matters do not cross**: scope, priority and deciding what to build stay with you.

## Configured elsewhere

- Talking to an agent by voice or in writing: [talking to the agents](falar-com-eles).
- What an agent can do on the canvas: [the agent calls colleagues](o-agente-chama-colegas).
- Storing an agent and bringing it back: [minimizing and the shelf](minimizar-e-a-estante).
