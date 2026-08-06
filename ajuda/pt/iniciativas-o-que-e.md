---
slug: iniciativas-o-que-e
titulo: O que é uma Iniciativa
resumo: O processo de trabalho do time escrito num arquivo do repositório, que o CanvasCode lê, desenha e conduz.
area: iniciativas
nivel: avancado
---

Uma **Iniciativa** é o processo que o seu time já segue, escrito num arquivo do repositório: as
etapas na ordem, quem faz cada uma, o que barra, e onde uma pessoa aprova. O CanvasCode lê esse
arquivo, desenha o processo e conduz as execuções.

**O app não implementa o processo de ninguém.** Quem executa continua sendo os comandos, os scripts e
os agentes que o projeto já tem. O arquivo é uma lente sobre eles, e se ele e os comandos
discordarem, os comandos ganham.

## O vocabulário

| Palavra | O que é |
|---|---|
| **Iniciativa** | O processo definido, num arquivo dentro do repositório |
| **Run** | Uma execução daquele processo, do começo ao fim |
| **Passo** | Uma etapa: um agente ou um comando, com o que entra e o que sai |
| **Portão** | Um comando que prova que o resultado do passo serve |
| **Revisão** | Um passo cuja saída é um veredito, e cujo efeito é mudar a rota |

## Para que serve

Para o trabalho que se repete e tem ordem: uma esteira de conteúdo, um fluxo de release, uma
apuração que sempre passa pelas mesmas cinco etapas com uma aprovação sua no meio.

Não serve para tarefa avulsa. Para pedir uma coisa a um agente, o caminho continua sendo o painel
dele ou a voz.

## O que muda em relação a mandar você mesmo

- **A ordem não se perde.** Cada passo recebe o que o anterior produziu, e um resumo de até três
  linhas com o que o artefato não diz: o risco que o agente viu e a decisão que ele tomou.
- **Quem diz que o passo acabou é o portão, não o agente.** O agente avisa que acha que terminou; o
  app roda o comando que prova, e se ele reprovar o trabalho volta com o motivo.
- **Quem revisa é sempre um agente novo**, porque revisar o próprio trabalho com a conversa ainda na
  cabeça é a revisão mais fraca que existe.
- **Quem conserta é o mesmo agente na primeira volta**, e um agente novo a partir da segunda.
- **Todo laço tem teto.** E um artefato idêntico ao da volta anterior para na hora, sem gastar a
  próxima volta.
- **Nenhum agente é acionado sem você escolher qual.** Todo botão que fala com agente abre o seletor
  antes e mostra o que vai ser mandado.

## Onde os arquivos ficam

- **A Iniciativa** fica em `.codecanvas/iniciativas/` dentro do repositório, e é versionada com o
  código: ela viaja para quem clonar o projeto.
- **As runs** ficam em `.codecanvas/runs/`, fora do git: são execução, não definição.

**Uma Iniciativa é por repositório.** Ela é feita dos comandos e scripts daquele projeto, e não é
reaproveitável em outro.

## O que dá para fazer em paralelo

Dentro de uma run, tudo é fila: um passo, um agente, uma entrada, uma saída. O paralelismo existe um
nível acima, em duas runs da mesma Iniciativa ao mesmo tempo, para comparar resultados.

## Por onde seguir

- Escrever uma: [escrever uma Iniciativa](iniciativas-escrever).
- Acompanhar as execuções: [o painel de Iniciativas](painel-iniciativas).
