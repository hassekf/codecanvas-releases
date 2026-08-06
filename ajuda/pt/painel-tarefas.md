---
slug: painel-tarefas
titulo: O painel de tarefas
resumo: A lista do projeto: anotar, mudar de estado, pôr prazo, o histórico de cada linha e o aviso de vencimento.
area: paineis
nivel: basico
---

Abra pelo `⌘K` com `tarefas`. O painel é um por canvas, e a lista pertence ao canvas: dois canvases
têm duas listas, mesmo apontando para a mesma pasta.

## Anotar

- **O campo do topo**: cria uma tarefa com o texto digitado. Enter e o botão **Anotar** fazem o
  mesmo. O prazo não é pedido aqui.

## A lista

Três seções, nesta ordem: **Fazendo**, **Abertas** e **Feitas**.

- **Fazendo** e **Abertas**: ordenadas pelo prazo mais próximo. Quem não tem prazo vai para o fim.
- **Feitas**: recolhida, com a contagem ao lado do título. Abre ao ser clicada, e também sozinha
  quando você conclui uma tarefa. Dentro dela, a mais recente vem primeiro.
- **O rodapé**: conta quantas tarefas estão pendentes e quantas venceram.

Cada linha mostra o texto da tarefa, o número dela, o estado escrito, o prazo, quem mexeu por último
e quantos comentários existem.

- **O número (`#3`)**: identifica a tarefa para a voz e para os agentes. Ele é único no canvas e
  nunca é reaproveitado, e reordenar a lista não renumera nada.
- **O nome de quem mexeu por último**: aparece só quando não foi você.
- **O último comentário**: fica visível na linha quando foi escrito por um agente ou pela Nina.
- **A barra na lateral esquerda**: marca a tarefa cujo prazo passou. Tarefa feita não recebe a barra,
  mesmo com o prazo vencido.

## Mudar o estado

- **O círculo à esquerda**: marca a tarefa como feita, e reabre a que já está feita. Ele não passa
  por "em andamento".
- **Começar** e **Pausar**: aparecem na linha sob o cursor. **Começar** move a tarefa aberta para em
  andamento; **Pausar** devolve a que está em andamento para aberta.
- **O estado escrito na linha**: é um menu, e leva a tarefa a qualquer um dos três estados.
- **O menu de contexto da linha**: repete os três estados, o prazo e **Apagar**.

## O prazo

O prazo é opcional. Pelo menu de contexto da linha, em **Prazo**:

- **Hoje**, **Amanhã** e **Semana que vem**: marcam o dia às 18h, e a linha mostra só o dia.
- **Tirar o prazo**: aparece apenas quando existe um prazo.

Prazo com hora se define pela voz ("entregar sexta às 17h") ou por um agente. Sem hora, o prazo cai
às 18h. O prazo vencido é escrito como "venceu às 13h" ou "venceu 4 de agosto".

## O verso da linha

Clicar na linha abre o verso, e clicar de novo o fecha.

- **Os comentários**: todos eles, com o autor e quando foram escritos.
- **Comentar…**: acrescenta um comentário seu.
- **Histórico**: cada criação, mudança de estado, reescrita, prazo, comentário, exclusão e
  restauração, com o nome de quem fez e quando. O nome fica gravado ali mesmo depois de o agente ser
  dispensado.

## A lixeira

- **Apagar**: manda a tarefa para a lixeira, e o histórico registra quem apagou. Um agente também
  apaga por aqui.
- **Lixeira**, no rodapé: mostra o que foi apagado, com **Restaurar** em cada linha.
- **Esvaziar**: apaga de vez o que está na lixeira. Nenhuma ferramenta de voz ou de agente alcança
  este botão.

## O aviso de prazo

Uma tarefa com prazo avisa três vezes: 1 hora antes, 30 minutos antes e no vencimento. Cada marco
avisa uma vez só, e reabrir o app não repete o que já foi dito. Quando mais de um marco chega junto,
só o mais urgente é falado.

- **O aviso vale para todos os canvases**, não só o que está à sua frente. Quando a tarefa é de outro
  projeto, o aviso diz de qual.
- **Clicar no aviso**: troca para o canvas daquela tarefa e abre o painel de tarefas.
- Ligar, desligar, calar e mandar ler em voz alta: [avisos e sons](avisos-e-sons).

## Quem mais escreve aqui

A Nina, por voz, e os agentes deste canvas. Eles criam tarefas, mudam o estado, comentam, reescrevem
o texto, mexem no prazo e apagam. Toda ação deles entra no histórico com o nome de quem fez, e o
comentário é o que aparece na linha quando eles concluem alguma coisa. Veja
[o agente usa as suas listas](o-agente-usa-suas-listas).

Em **Configurações → Saudação**, **Bom-dia ao abrir** com **Falar das tarefas** ligado conta, na
primeira abertura do dia, o que venceu e o que vence hoje nas suas listas.

Para texto que você quer guardar em vez de fazer, use [o painel de notas](painel-notas).
