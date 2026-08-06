---
slug: o-que-ela-consegue-fazer
titulo: O que dá para pedir
resumo: O repertório da Nina por assunto: a frase que você diz e o que acontece no canvas.
area: nina
nivel: basico
---

Tudo aqui vale nas três formas de mandar: [a conversa por voz](falar-com-a-nina) (⌥C), [o modo
comando](o-modo-comando) (⌥X) e [a conversa escrita](a-nina-por-texto) (⌘J). Os grupos de
ferramentas se desligam em **Configurações → Ferramentas**, e cada um mostra ali quantos tokens custa
por troca.

## Agentes

| Você diz | O que acontece |
|---|---|
| *"abre um agente"* · *"sobe dois agentes"* | Nascem no canvas, já com nome |
| *"cria um agente do Codex"* | O mesmo, no CLI que você nomear |
| *"chama o Hermes de volta"* | O agente dispensado volta com a conversa inteira |
| *"ei Freya, roda os testes"* | A tarefa vai para a Freya, do jeito que você falou |
| *"manda alguém investigar o build lento"* | Ela escolhe um agente livre, ou cria um |
| *"fecha a Freya"* · *"dispensa o Apolo"* | O painel sai da tela e a memória fica guardada |
| *"manda o Apolo continuar"* | O agente caído retoma de onde parou |
| *"só quando o Claude voltar ao ar"* | A retomada espera o provedor sair da instabilidade |
| *"deixa o Apolo falar com a Gerda do backend"* | Abre a conversa entre agentes de projetos diferentes |

Falar com um agente não cria ninguém: um agente dispensado volta pelo nome, com a conversa inteira.
Pedidos que exigem trabalho real (pesquisar, comparar, escrever código) são entregues a um agente.

## Saber o que está acontecendo

| Você diz | O que acontece |
|---|---|
| *"como estamos?"* | Ela conta o assunto de cada agente |
| *"quais agentes existem?"* | Os que estão na tela e os guardados |
| *"quem está trabalhando agora?"* | Só os que estão em tarefa |
| *"o que o Apolo andou fazendo?"* | A tarefa dele, o que fez e o que respondeu por último |
| *"quem foi que mexeu no pagamento?"* | Procura o assunto no histórico de todos, inclusive dispensados |
| *"mostra o status"* · *"esconde o status"* | Vira e desvira os painéis |
| *"o que ele perguntou?"* · *"quais são as opções?"* | Lê a pergunta pendente de um agente |
| *"a segunda"* · *"usa o que já está no docker compose"* | Responde a pergunta dele, pela opção ou com texto seu |

"Mostra" vira a tela; "me diz" vira uma frase falada. Quando a sua resposta não casa com nenhuma
opção da pergunta de um agente, ela repete a pergunta em vez de escolher por você.

## Painéis e arranjo

| Você diz | O que acontece |
|---|---|
| *"abre o git"* · *"abre um terminal"* · *"abre a mídia"* | O painel nasce no canvas |
| *"abre o browser no localhost:3000"* | Um navegador já naquele endereço |
| *"me mostra o README"* | O arquivo abre num painel |
| *"fecha o browser"* · *"fecha os agentes"* · *"fecha tudo"* | Fecha por nome, por tipo, ou a área inteira |
| *"coloca o browser em foco"* · *"tira o foco"* | Destaca um painel e devolve os outros à grade |
| *"me leva até a Gerda"* | A câmera vai até ela, trocando de projeto e de área se precisar |
| *"organiza as janelas"* · *"põe em duas colunas"* | Arruma o canvas, ou troca o arranjo da grade |
| *"salva esse arranjo como revisão de PR"* | Guarda o arranjo com esse nome |
| *"volta pro arranjo de pareamento"* | Restaura um arranjo guardado, sem abrir nem fechar painel |

Fechar cobre um painel pelo nome, vários, todos de um tipo ou o canvas inteiro. Veja
[organizar sozinho](organizar-sozinho).

## Projetos e áreas

| Você diz | O que acontece |
|---|---|
| *"muda pro projeto platform"* | Troca de canvas |
| *"cria um canvas em /Users/eu/www/site"* | Cria um projeto naquela pasta |
| *"cria uma área pro front"* | Nasce uma aba nova neste canvas |
| *"vai pra área do back"* · *"próxima área"* | Troca de aba |
| *"manda o Marshall pra área do back"* | O agente vai vivo, no meio do que estiver fazendo |

Projeto é outra pasta e outro elenco; área é outra aba do mesmo projeto. Veja
[áreas de trabalho](areas-de-trabalho) e [vários canvases](varios-canvases).

## Tarefas

| Você diz | O que acontece |
|---|---|
| *"anota aí que eu preciso arrumar o login"* | Cria a tarefa |
| *"bota na lista: entregar o relatório sexta"* | Cria com prazo |
| *"o que falta neste projeto?"* · *"o que eu tenho pra hoje?"* | Lê o que está aberto |
| *"marca a três como feita"* | Muda o estado da tarefa 3 |
| *"muda o prazo da dois pra amanhã"* | Reagenda |
| *"comenta na do relatório que já testei"* | Escreve um comentário assinado |
| *"tira aquela do login da lista"* | Manda para a lixeira |

"Já fiz" marca como feita; apagar só acontece quando você manda apagar, e a tarefa vai para a
lixeira do [painel de tarefas](painel-tarefas).

## Notas

| Você diz | O que acontece |
|---|---|
| *"guarda esse endereço numa nota"* | Cria uma nota |
| *"lê a nota do deploy"* | Ela lê o texto inteiro daquela nota |
| *"adiciona na nota do deploy que a porta é 8080"* | Acrescenta ao fim, sem reescrever o que estava lá |

Ela cria, acrescenta ao fim e renomeia. Apagar uma nota é só pelo [painel](painel-notas).

## Recados

| Você diz | O que acontece |
|---|---|
| *"quem são meus contatos?"* | Lista quem você já adicionou |
| *"o que chegou de recado?"* | Lê os não lidos |
| *"avisa o Pedro que o deploy saiu"* | Manda um recado novo |
| *"responde pra ela que eu vejo amanhã"* | Responde o último que chegou |

Recado vai para outra pessoa, em outro computador. Veja [os recados](painel-recados).

## Repositório e issues

| Você diz | O que acontece |
|---|---|
| *"como está o git?"* | Branch, o que mudou e os últimos commits |
| *"o que mudou e ainda não foi commitado?"* | Os arquivos sujos, com quem mexeu em cada um |
| *"quais PRs estão abertas?"* · *"quais esperam a minha revisão?"* | Lista as pull requests |
| *"aprova a 42"* | Publica a aprovação no GitHub |
| *"comenta na 42 que falta o teste"* | Comenta sem aprovar |
| *"quais issues estão abertas?"* | Lista as issues |
| *"cria um bug com esse erro do console"* | Abre uma issue |
| *"renomeia a issue 12"* · *"fecha a 12"* · *"reabre a 12"* | Mexe naquela issue |
| *"pega a primeira issue e começa"* | Abre um agente com a issue como tarefa |
| *"manda esse bug pro Hermes"* | Entrega a issue a um agente já aberto |

A leitura do repositório diz qual agente mexeu em cada arquivo. Veja [o painel do Git](painel-git).

## Jira e Confluence

| Você diz | O que acontece |
|---|---|
| *"o que tem no board?"* · *"o que tá em andamento?"* | Lê o quadro do projeto conectado |
| *"cria uma tarefa pra revisar o login"* | Cria um cartão no Jira |
| *"move a PROJ-12 pra pronto"* | Muda o cartão de coluna |
| *"o que o Confluence diz sobre o fluxo de pagamento?"* | Busca na base de documentação |

Cada projeto fala com a própria conta. Veja [Jira e Confluence](jira-e-confluence).

## Skills e MCP

| Você diz | O que acontece |
|---|---|
| *"quais skills este projeto tem?"* | Lista as skills à mão deste canvas |
| *"desativa a skill de revisão aqui"* | Desliga só neste projeto |
| *"procura uma skill de testes"* · *"instala essa aí"* | Busca no registro público e instala |
| *"quais MCPs estão ligados?"* · *"procura um MCP de Postgres"* | O mesmo, para servidores de ferramentas |

Instalar deixa código de terceiros rodar nos seus agentes, então esse pedido passa por uma
confirmação sua. Veja [skills e MCP](skills-e-mcp).

## Aparência e imagens

| Você diz | O que acontece |
|---|---|
| *"troca o tema pra forja"* · *"deixa em ameixa"* | Troca o tema deste projeto |
| *"põe um fundo de floresta"* | Pinta um papel de parede novo |
| *"procura outro"* | Troca pelo próximo candidato, sem repetir a descrição |
| *"tira o fundo"* | Devolve a paisagem do tema |
| *"gera uma imagem de um gato astronauta"* | A imagem nasce no canvas e vai para a galeria |
| *"cria três ilustrações de uma floresta"* | O mesmo, na quantidade que você pedir |
| *"quantas imagens tem no canvas?"* | Ela conta o que está colado ali |

Fundo é o papel de parede; imagem gerada aparece no canvas e fica na [galeria](painel-galeria). As
duas levam algum tempo, e o app avisa quando ficam prontas. Veja [aparência](aparencia).

## Mídia, webcam e gravação

| Você diz | O que acontece |
|---|---|
| *"põe pra tocar"* · *"pausa aí"* | Comanda o que já está no painel de mídia |
| *"muda pra música"* | Troca entre vídeo e música |
| *"minimiza o vídeo, quero só o áudio"* | Encolhe numa cápsula, com o som seguindo |
| *"modo cinema"* | Esconde a página e deixa só o vídeo |
| *"abre a webcam"* · *"espelha a imagem"* · *"usa a câmera do iPhone"* | Abre e ajusta a webcam |
| *"começa a gravar"* · *"pausa a gravação"* · *"para de gravar"* | Comanda a gravação de tela |
| *"deixa a janela em vertical"* · *"põe em paisagem"* | Redimensiona a janela do app para gravar |

Ela comanda o que já está tocando; escolher o vídeo é pedido que vai para um agente. Veja
[o painel de mídia](painel-midia), [a webcam](painel-webcam-e-avatar) e
[a gravação](painel-gravacao).

## Agenda e reuniões

| Você diz | O que acontece |
|---|---|
| *"o que eu tenho hoje?"* · *"qual a próxima reunião?"* | Lê a sua agenda |
| *"do que é a reunião das três?"* · *"quem vai estar nela?"* | Detalha um compromisso |
| *"entra na reunião"* · *"abre o Meet"* | Abre a chamada e liga o modo reunião |
| *"fica quieta um pouco"* | Liga o modo reunião sem reunião nenhuma |
| *"acabou a reunião"* | Desliga o modo reunião |

Ela lê o calendário e entra na chamada. Não cria, não move e não cancela compromisso. Veja
[agenda e reuniões](agenda-e-reunioes).

## Ditado que foi para o agente errado

| Você diz | O que acontece |
|---|---|
| *"aquilo da migração, joga pro Hermes"* | O texto que você já ditou vai para outro agente |
| *"mandei errado, reenvia o último pro Apolo"* | O mesmo, com o último ditado |

O texto original é reaproveitado; você não precisa repetir a frase. Veja [ditado](ditado).

## Encerrar

*"pode dormir"*, *"tchau"*, *"valeu"* e *"chega"* encerram a conversa por voz. Os agentes continuam
trabalhando.
