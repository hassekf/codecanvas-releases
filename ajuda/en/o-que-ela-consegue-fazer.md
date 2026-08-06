---
slug: o-que-ela-consegue-fazer
titulo: What you can ask for
resumo: Nina's repertoire by subject: the sentence you say, and what happens on the canvas.
area: nina
nivel: basico
---

Everything here works in the three ways of ordering: [the voice conversation](falar-com-a-nina) (⌥C),
[command mode](o-modo-comando) (⌥X) and [the written conversation](a-nina-por-texto) (⌘J). The tool
groups are turned off in **Settings → Tools**, and each one shows there how many tokens it costs per
exchange.

**The example sentences below stay in Portuguese, on purpose.** Voice commands are interpreted in
Portuguese, so a translated example would be a sentence that does not work. Say them as they are
written; the column beside them, in English, tells you what happens.

## Agents

| You say | What happens |
|---|---|
| *"abre um agente"* · *"sobe dois agentes"* | They are born on the canvas, already named |
| *"cria um agente do Codex"* | The same, in whichever CLI you name |
| *"chama o Hermes de volta"* | The dismissed agent comes back with the whole conversation |
| *"ei Freya, roda os testes"* | The task goes to Freya, worded the way you said it |
| *"manda alguém investigar o build lento"* | She picks a free agent, or creates one |
| *"fecha a Freya"* · *"dispensa o Apolo"* | The panel leaves the screen and the memory is kept |
| *"manda o Apolo continuar"* | The agent that fell resumes from where it stopped |
| *"só quando o Claude voltar ao ar"* | The resume waits for the provider to come out of the outage |
| *"deixa o Apolo falar com a Gerda do backend"* | Opens the conversation between agents of different projects |

Talking to an agent creates nobody: a dismissed agent comes back by name, with the whole
conversation. Requests that take real work (searching, comparing, writing code) are handed to an
agent.

## Knowing what is going on

| You say | What happens |
|---|---|
| *"como estamos?"* | She tells you what each agent is working on |
| *"quais agentes existem?"* | The ones on the screen and the ones put away |
| *"quem está trabalhando agora?"* | Only the ones on a task |
| *"o que o Apolo andou fazendo?"* | Apolo's task, the work done, and the last answer given |
| *"quem foi que mexeu no pagamento?"* | Searches the subject in everyone's history, dismissed agents included |
| *"mostra o status"* · *"esconde o status"* | Flips the panels over and back |
| *"o que ele perguntou?"* · *"quais são as opções?"* | Reads an agent's pending question |
| *"a segunda"* · *"usa o que já está no docker compose"* | Answers that question, by option or with text of your own |

"Mostra" changes the screen; "me diz" produces a spoken sentence. When your answer matches none of
the options in an agent's question, she repeats the question instead of choosing for you.

## Panels and layout

| You say | What happens |
|---|---|
| *"abre o git"* · *"abre um terminal"* · *"abre a mídia"* | The panel is born on the canvas |
| *"abre o browser no localhost:3000"* | A browser already at that address |
| *"me mostra o README"* | The file opens in a panel |
| *"fecha o browser"* · *"fecha os agentes"* · *"fecha tudo"* | Closes by name, by type, or the whole workspace |
| *"coloca o browser em foco"* · *"tira o foco"* | Highlights one panel and gives the others back to the grid |
| *"me leva até a Gerda"* | The camera travels to Gerda, switching project and workspace if it has to |
| *"organiza as janelas"* · *"põe em duas colunas"* | Tidies up the canvas, or changes the grid layout |
| *"salva esse arranjo como revisão de PR"* | Saves the layout under that name |
| *"volta pro arranjo de pareamento"* | Restores a saved layout, without opening or closing any panel |

Closing covers one panel by name, several, all of a type or the whole canvas. See
[tidying up on its own](organizar-sozinho).

## Projects and workspaces

| You say | What happens |
|---|---|
| *"muda pro projeto platform"* | Switches canvas |
| *"cria um canvas em /Users/eu/www/site"* | Creates a project in that folder |
| *"cria uma área pro front"* | A new tab is born in this canvas |
| *"vai pra área do back"* · *"próxima área"* | Switches tab |
| *"manda o Marshall pra área do back"* | The agent moves while running, in the middle of whatever it is doing |

A project is another folder with another cast; a workspace is another tab of the same project. See
[workspaces](areas-de-trabalho) and [several canvases](varios-canvases).

## Tasks

| You say | What happens |
|---|---|
| *"anota aí que eu preciso arrumar o login"* | Creates the task |
| *"bota na lista: entregar o relatório sexta"* | Creates it with a due date |
| *"o que falta neste projeto?"* · *"o que eu tenho pra hoje?"* | Reads what is open |
| *"marca a três como feita"* | Changes the state of task 3 |
| *"muda o prazo da dois pra amanhã"* | Reschedules it |
| *"comenta na do relatório que já testei"* | Writes a signed comment |
| *"tira aquela do login da lista"* | Sends it to the bin |

"Já fiz" marks it as done; deleting only happens when you say so, and the task goes to the bin in
[the task panel](painel-tarefas).

## Notes

| You say | What happens |
|---|---|
| *"guarda esse endereço numa nota"* | Creates a note |
| *"lê a nota do deploy"* | She reads out the whole text of that note |
| *"adiciona na nota do deploy que a porta é 8080"* | Appends to the end, without rewriting what was there |

She creates, appends to the end and renames. Deleting a note is only done in
[the panel](painel-notas).

## Messages

| You say | What happens |
|---|---|
| *"quem são meus contatos?"* | Lists the people you have added |
| *"o que chegou de recado?"* | Reads the unread ones |
| *"avisa o Pedro que o deploy saiu"* | Sends a new message |
| *"responde pra ela que eu vejo amanhã"* | Replies to the last one that arrived |

A message goes to another person, on another computer. See [messages](painel-recados).

## Repository and issues

| You say | What happens |
|---|---|
| *"como está o git?"* | The branch, what changed and the latest commits |
| *"o que mudou e ainda não foi commitado?"* | The dirty files, with who touched each one |
| *"quais PRs estão abertas?"* · *"quais esperam a minha revisão?"* | Lists the pull requests |
| *"aprova a 42"* | Publishes the approval on GitHub |
| *"comenta na 42 que falta o teste"* | Comments without approving |
| *"quais issues estão abertas?"* | Lists the issues |
| *"cria um bug com esse erro do console"* | Opens an issue |
| *"renomeia a issue 12"* · *"fecha a 12"* · *"reabre a 12"* | Acts on that issue |
| *"pega a primeira issue e começa"* | Opens an agent with the issue as its task |
| *"manda esse bug pro Hermes"* | Hands the issue to an agent that is already open |

Reading the repository tells you which agent touched each file. See [the Git panel](painel-git).

## Jira and Confluence

| You say | What happens |
|---|---|
| *"o que tem no board?"* · *"o que tá em andamento?"* | Reads the board of the connected project |
| *"cria uma tarefa pra revisar o login"* | Creates a card in Jira |
| *"move a PROJ-12 pra pronto"* | Moves the card to another column |
| *"o que o Confluence diz sobre o fluxo de pagamento?"* | Searches the documentation base |

Each project talks to its own account. See [Jira and Confluence](jira-e-confluence).

## Skills and MCP

| You say | What happens |
|---|---|
| *"quais skills este projeto tem?"* | Lists the skills this canvas has at hand |
| *"desativa a skill de revisão aqui"* | Turns it off in this project only |
| *"procura uma skill de testes"* · *"instala essa aí"* | Searches the public registry and installs |
| *"quais MCPs estão ligados?"* · *"procura um MCP de Postgres"* | The same, for tool servers |

Installing lets third-party code run in your agents, so that request goes through a confirmation of
yours. See [skills and MCP](skills-e-mcp).

## Appearance and images

| You say | What happens |
|---|---|
| *"troca o tema pra forja"* · *"deixa em ameixa"* | Changes this project's theme |
| *"põe um fundo de floresta"* | Paints a new wallpaper |
| *"procura outro"* | Swaps it for the next candidate, without repeating the description |
| *"tira o fundo"* | Gives the theme's own landscape back |
| *"gera uma imagem de um gato astronauta"* | The image is born on the canvas and goes to the gallery |
| *"cria três ilustrações de uma floresta"* | The same, in the quantity you ask for |
| *"quantas imagens tem no canvas?"* | She counts what is pinned there |

The background is the wallpaper; a generated image appears on the canvas and stays in
[the gallery](painel-galeria). Both take a while, and the app tells you when they are ready. See
[appearance](aparencia).

## Media, webcam and recording

| You say | What happens |
|---|---|
| *"põe pra tocar"* · *"pausa aí"* | Controls what is already in the media panel |
| *"muda pra música"* | Switches between video and music |
| *"minimiza o vídeo, quero só o áudio"* | Shrinks it into a capsule, with the sound following |
| *"modo cinema"* | Hides the page and leaves only the video |
| *"abre a webcam"* · *"espelha a imagem"* · *"usa a câmera do iPhone"* | Opens and adjusts the webcam |
| *"começa a gravar"* · *"pausa a gravação"* · *"para de gravar"* | Controls the screen recording |
| *"deixa a janela em vertical"* · *"põe em paisagem"* | Resizes the app window for recording |

She controls what is already playing; choosing the video is a request that goes to an agent. See
[the media panel](painel-midia), [the webcam](painel-webcam-e-avatar) and
[recording](painel-gravacao).

## Calendar and meetings

| You say | What happens |
|---|---|
| *"o que eu tenho hoje?"* · *"qual a próxima reunião?"* | Reads your calendar |
| *"do que é a reunião das três?"* · *"quem vai estar nela?"* | Details one appointment |
| *"entra na reunião"* · *"abre o Meet"* | Opens the call and turns meeting mode on |
| *"fica quieta um pouco"* | Turns meeting mode on with no meeting at all |
| *"acabou a reunião"* | Turns meeting mode off |

She reads the calendar and joins the call. She does not create, move or cancel appointments. See
[calendar and meetings](agenda-e-reunioes).

## A dictation that went to the wrong agent

| You say | What happens |
|---|---|
| *"aquilo da migração, joga pro Hermes"* | The text you already dictated goes to another agent |
| *"mandei errado, reenvia o último pro Apolo"* | The same, with the last dictation |

The original text is reused; you do not have to say it again. See [dictation](ditado).

## Ending

*"pode dormir"*, *"tchau"*, *"valeu"* and *"chega"* end the voice conversation. The agents keep
working.
