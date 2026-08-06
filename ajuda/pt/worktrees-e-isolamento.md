---
slug: worktrees-e-isolamento
titulo: Cada agente na sua cópia
resumo: O isolamento por worktree, o texto que instrui os agentes, a barra de frentes e a entrega de uma frente pronta.
area: agentes
nivel: avancado
---

## O isolamento

Em **Configurações → Agentes → Isolamento por worktree**, ligado por padrão.

- **Isolamento por worktree**: instrui cada agente a criar a própria worktree do repositório e a
  commitar na branch dele antes de escrever qualquer arquivo. Desligado, todos os agentes escrevem no
  mesmo diretório.
- **A instrução vale para os próximos agentes.** Ela entra no prompt de sistema no nascimento do
  processo, e nenhum agente que já está de pé muda de comportamento quando você salva.
- **É instrução, e não trava do app.** Um agente decide segui-la, e o protocolo dispensa a worktree
  em tarefa que só lê e em projeto sem repositório Git.

## O texto que os agentes leem

- **Personalizar instruções…**: abre o editor do protocolo, logo abaixo do interruptor. Depois de
  editado, o botão passa a dizer **Editar instruções…**.
- **{nome}**: o marcador que vira o identificador de cada agente, e portanto a branch e a pasta dele.
  Sem ele, o editor alerta e permite salvar assim mesmo, e os agentes disputam a mesma
  branch.
- **Restaurar padrão**: repõe o texto de fábrica no editor, e fica indisponível quando o que está
  ali já é o padrão.
- **Concluir** com o texto vazio, ou idêntico ao padrão, desfaz a personalização: o projeto volta a
  acompanhar o texto padrão em vez de guardar uma cópia dele.

Cada projeto pode discordar do ajuste do app, em **Editar o projeto → Agentes → Isolamento por
worktree**:

- **Seguir o ajuste global**, **Ligado neste projeto** ou **Desligado neste projeto**.
- **Instruções próprias deste projeto**: aparece com o isolamento ligado e substitui o texto global
  só neste canvas.

## A barra de frentes

`⌘⇧F` abre e fecha a barra da esquerda. A tecla se troca em Configurações → Atalhos.

Cada seção é uma área de trabalho, inclusive as que não estão à vista, e dentro dela vem uma linha
por agente.

- **A linha de uma frente** traz o nome do agente, as linhas somadas e removidas, a branch, o estágio
  e quantos commits do destino ela ainda não viu. Clicar leva a câmera até o agente.
- **A etiqueta "só branch"** marca o trabalho que existe como branch e já não tem diretório.
- **Os agentes sem frente também aparecem**, com o estado atual: quem só leu código não tem branch
  nem worktree.
- **A linha do topo** é a base do canvas, com quantos arquivos estão fora de commit ali.
- **O olho do cabeçalho** mostra e esconde o assunto anotado por cada agente.
- **O botão ao lado dele** alterna entre a barra flutuante e a barra encaixada na lateral, com o
  canvas ao lado. Ela nasce flutuante.
- **Os arquivos disputados** ficam no pé da lista: os que mais de uma frente está tocando agora,
  commitados ou não.
- **O rodapé** conta quantas frentes estão prontas para integrar e quantas estão em revisão, e o
  botão ao lado relê o repositório do zero, sem aproveitar o que a barra já sabia.
- **Um repositório grande não é lido inteiro.** As branches com worktree entram sempre, e do resto
  entram as mais recentes. A barra diz quantas ficaram de fora.
- **O menu de contexto de uma linha** leva até o agente, ou chama um agente para uma worktree sem
  dono, e copia o caminho da worktree, o nome da branch, ou abre a pasta no Finder.

## O que a barra lista

Em **Configurações → Interface → Barra de frentes**.

- **Mostrar branches sem worktree**, ligado: também aparecem as branches cujo diretório de trabalho
  já foi removido. Desligado, uma branch nesse estado fica invisível.
- **Mostrar as já integradas**, desligado: as frentes que já estão inteiras na base saem da lista.
- **Esconder as abas de área quando ela estiver encaixada**, desligado: as abas do topo somem e a
  barra passa a trocar de área, renomear e criar. Só funciona com a barra encaixada, e fica
  indisponível enquanto ela estiver flutuando.
- **Agrupar os agentes em abas**: numa área com mais de um agente, eles dividem um painel com abas no
  alto. O menu de contexto de cada área decide por conta própria.

## Entregar uma frente

O botão de entrega aparece na linha das frentes prontas, publicadas ou em revisão, e nas outras só
quando o cursor passa por cima.

- **O botão não integra nada**: ele manda um recado ao agente que está dentro daquela worktree.
- **O rótulo diz o destino** apurado no histórico da própria branch: mergear naquele branch, abrir
  pull request para ele, ou apenas avisar que terminou.
- **O menu do botão** troca o modo. A escolha vale para aquele destino e fica gravada.
- **Retomar**, nas frentes paradas ou vazias sem ninguém dentro: abre um agente novo e o manda entrar
  naquela worktree. O botão não aparece quando a frente já tem agente.

Em **Configurações → Interface**:

- **Como entregar uma frente pronta**: escolhe o modo padrão de todos os destinos de todos os
  projetos. Deduzir de cada destino olha como o trabalho entrou naquele branch antes e sugere o
  mesmo. A escolha feita no menu da barra manda por cima, e só naquele destino.
- **Editar o recado…**: reescreve o texto que o botão envia. Os três marcadores viram o nome da
  branch, o destino e o verbo do modo escolhido, e sem o marcador da ação o recado não diz o que
  fazer.

## Quando vários terminam ao mesmo tempo

Um agente que acabou de integrar pode passar a vez ao próximo da fila, e o próximo recebe no painel
dele o aviso de que chegou a vez. Isso só alcança agentes vivos deste canvas: quem foi dispensado ou
está noutro canvas não é acordado.

## Configurado em outra tela

- As áreas de trabalho que viram seções da barra: [áreas de trabalho](areas-de-trabalho).
- O estado de cada agente: [saber o que fazem](saber-o-que-fazem).
- O repositório no canvas: [o agente e o git](o-agente-e-o-git).
