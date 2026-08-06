---
slug: o-modo-comando
titulo: Command mode
resumo: Holding ⌥X and speaking an order: what it accepts, what it refuses and how the sentence becomes action.
area: nina
nivel: basico
---

**⌥X**: hold the key, speak the order, release. The key changes in **Settings → Shortcuts**, on the
"Comandar" row.

The command runs and confirms in one short sentence. It does not open a conversation and does not
listen for your reply. To talk, use [Nina by voice](falar-com-a-nina) (⌥C); to write text inside an
agent, use [dictation](ditado) (⌥D).

**Command mode understands Portuguese**, and only Portuguese. The app interface speaks English,
Portuguese and Spanish, and [dictation](ditado) follows the chosen language, but spoken orders are
interpreted in Portuguese. An order spoken in another language is not carried out, so the examples
below are the sentences that work.

## What you can order

The same tools Nina has, listed in [what she can do](o-que-ela-consegue-fazer). Examples that work as
written:

```
"abre um agente"                      "sobe dois agentes"
"ei Freya, roda os testes"            "pede pro Apolo revisar o login"
"chama a Freya de volta"              "quais agentes existem?"
"quem foi que mexeu no pagamento?"    "como estamos?"
"abre o git"                          "fecha o browser"
"coloca o browser em foco"            "me leva até a Gerda"
"anota aí que eu preciso arrumar o login"
"organiza as janelas uma embaixo da outra"
"troca o tema pra forja"              "põe um fundo de floresta"
```

### Several orders in one sentence

One sentence can carry as many orders as you speak, and they run in the order they appear:

```
"fecha o Apolo e organiza em duas colunas"
"bom dia! fecha a Gerda, abre dois agentes, põe em duas colunas e mostra o status"
```

Greetings do not count as orders, and the same order said twice over ("minimiza o vídeo, quero só o
áudio") is still one.

### When there is no order at all

Sentences like "testando, você está me ouvindo?" get a short answer and nothing happens on screen.
Not understanding and there being no order are different things: in the second case the app answers
in one sentence instead of inventing an action.

## What it refuses

Every order goes through a check before running, and four things are impossible:

- **Closing without a closing verb in your sentence** ("fecha", "tira", "apaga", "dispensa",
  "limpa").
- **Closing everything without the word "tudo"**.
- **Creating an agent without a creation verb.** Saying the word "agente" is not enough: "põe os
  agentes em três colunas" creates nobody.
- **Sending anything to an agent whose name you did not say.**

When one of these guards blocks something, the reason is recorded in the voice log, in Settings →
Diagnostics.

## How the sentence becomes action

Your speech is transcribed on your own Mac, and only the text leaves it. The text is interpreted by
the model chosen in **Settings → Voice → Command model**, which depends on the OpenAI key. Without a
key, without a network, or with no answer to the request, a model on your Mac takes over, and after
it a keyword router.

Command mode costs a fraction of a conversation turn. See
[what it costs](quanto-custa).

## What you see and hear

- While the key is held, a small window shows the text being transcribed.
- When the order goes to an agent, a spark crosses the canvas to that agent's panel, showing which
  agent the app sent it to.
- The confirmation is spoken with the natural voice, or with the system voice when that one is off.
  The voice starts about a second later; the action has already happened by then.
- **Esc** cancels the command in progress.
