---
slug: areas-de-trabalho
titulo: Áreas de trabalho
resumo: As abas do canvas: o que cada uma guarda, como trocar, e como levar painéis de uma para a outra.
area: canvas
nivel: basico
---

As áreas de trabalho são as abas no alto do canvas. Elas dividem os painéis de um projeto; a pasta,
o Git e o elenco de agentes continuam sendo os mesmos. Para trabalhar em outra pasta, o que se cria
é outro canvas: veja [vários canvases](varios-canvases).

Cada área guarda os seus painéis, o modo e o arranjo da mesa, a posição e o zoom da câmera, e a
escolha de agrupar ou não os agentes em abas.

## Criar e nomear

- **A bolinha `+`**, ao lado das abas: cria uma área e já abre o nome para você digitar. Enter ou
  clicar fora confirma o nome; Esc cancela a edição e mantém o anterior.
- **Clicar na aba em que você já está**: abre o nome dela para edição.
- **Menu do botão direito da aba → Renomear…**: o mesmo.
- **Por voz**: *"cria uma área pro front"*.

A barra de abas aparece mesmo com uma área só. Ela some quando a barra de frentes está encaixada e
a opção **Esconder as abas de área quando ela estiver encaixada** está ligada, em
**Configurações → Interface**; ali a própria barra de frentes lista as áreas e troca entre elas.

## Trocar de área

- **Clique na aba**.
- **⌃⇥ e ⌃⇧⇥**: a próxima e a anterior, dando a volta no fim. Com o cursor dentro de um agente,
  essas duas teclas podem ser consumidas pelo terminal antes de chegar ao canvas.
- **Por voz**: *"vai pra área do back"*. *"Muda pro projeto X"* é outra coisa: troca de canvas.

Nada é encerrado na troca. Os painéis da área atual saem da tela e os da outra aparecem; o agente
que estava compilando continua compilando.

- **O ponto na aba**: aparece nas abas que não são a sua, e diz que há alguém esperando você ou
  alguém trabalhando naquela área.
- **A aba pisca** quando um agente termina ou passa a esperar você numa área fora da vista. Isso se
  desliga em **Configurações → Interface**, no controle **Destacar a aba da área ao terminar**.

## Levar um painel para outra área

- **Arrastar o painel até a aba de destino**: a aba acende quando o cursor chega nela, e uma ficha no
  cursor diz o que vai ser levado. Com vários painéis selecionados, vão todos, e as imagens
  selecionadas do canvas vão junto.
- **Menu do botão direito do painel → Mover para a área**: só aparece com mais de uma área.
- **Por voz**: *"manda o Marshall pra área do back"*.

O agente vai vivo, no meio do que estiver fazendo.

## Apagar uma área

**Menu do botão direito da aba → Apagar “nome”**, disponível só a partir de duas áreas. Nenhum painel
é fechado: eles passam para a área vizinha com os agentes vivos dentro, e o aviso diz quantos foram
e para onde.

## Os agentes numa aba só

**Menu do botão direito da aba → Agrupar os agentes em abas**: os agentes daquela área passam a
dividir um painel, com uma fileira de abas no alto; o escolhido ocupa o painel e os outros continuam
trabalhando escondidos. **Separar os agentes em painéis** desfaz.

- A decisão é de cada área e manda por cima do padrão do app, que fica em
  **Configurações → Interface**, no controle **Agrupar os agentes em abas**.
- **Seguir o padrão do app** só aparece quando aquela área discorda do padrão, e devolve a decisão a
  ele.
- Arrastar um agente sobre o cabeçalho de outro junta os dois num grupo avulso, que convive com o
  agrupamento da área.

## O que atravessa as áreas

- **O ⌘K** acha painéis de todas as áreas. Veja [busca e comandos](busca-e-comandos).
- **A lista de agentes** e as perguntas do tipo *"quem está trabalhando?"* respondem pelo projeto
  inteiro.
- **A barra de frentes** (**⌘⇧F**) mostra as áreas como seções. Veja
  [worktrees e isolamento](worktrees-e-isolamento).
- **A estante** mostra uma área por vez, escolhida no seletor do topo. Veja
  [minimizar e a estante](minimizar-e-a-estante).
- **Fechar por tipo**, por voz, age só na área aberta; fechar pelo nome alcança qualquer área. Veja
  [os painéis e a mesa](os-paineis-e-a-mesa).
