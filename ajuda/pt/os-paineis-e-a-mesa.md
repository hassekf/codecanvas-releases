---
slug: os-paineis-e-a-mesa
titulo: Os painéis e a mesa
resumo: Abrir, mover, redimensionar, selecionar e fechar painéis, e os dois modos em que a mesa se arruma.
area: canvas
nivel: basico
---

## Abrir um painel

- **⌘K** e o nome do que você quer: terminal, navegador, git, notas. Veja
  [busca e comandos](busca-e-comandos).
- **Os botões da barra de comando**, no rodapé: **Buscar no canvas**, **Novo agente** e
  **Novo browser**.
- **⌘N** abre um agente, **⌘⇧N** abre um agente do Codex (só com o Codex ligado em
  **Configurações → Provedores**) e **⌘T** abre um terminal sem agente. As três funcionam mesmo com
  o cursor dentro de outro agente.
- **Por voz**: *"abre um navegador"*, *"abre o git"*.

Os agentes também abrem painéis por conta própria. Veja
[o agente mexe no canvas](o-agente-mexe-no-canvas).

## O cabeçalho

Arrastar pelo cabeçalho move o painel. Clicar nele traz o painel para a frente e o seleciona.

- **Soltar da grade**: tira o painel do arranjo automático e lhe dá posição e tamanho próprios, sobre
  a grade. Só existe na grade automática, e um painel solto não pode estar em destaque ao mesmo
  tempo.
- **Destacar este painel**: põe este painel grande à esquerda e empilha os demais numa coluna à
  direita. Não aparece em painel solto da grade. Por voz, *"foco no Perseu"* e *"desfoca"* fazem o
  mesmo.
- **Minimizar**: guarda o painel na [estante](minimizar-e-a-estante), com o conteúdo vivo.
- **Fechar**: tira o painel do canvas. Um agente fechado é dispensado, não apagado: veja
  [criar e fechar](criar-e-fechar).

O clique direito no cabeçalho abre o menu do painel: escrever um assunto fixo para ele, trocar a
conta do agente, minimizar, e **Mover para a área**, que só aparece quando o projeto tem mais de uma
[área de trabalho](areas-de-trabalho).

## Os dois modos da mesa

O seletor fica na barra de comando, e a escolha é **de cada área de trabalho**: a grade do front não
mexe na do back.

- **Grade automática**: o app decide posição e tamanho de todos. Abrir ou fechar um painel
  redistribui os demais na hora. Arrastar um painel e soltá-lo perto de outro troca os dois de
  lugar, dentro da mesma área.
- **Canvas livre**: a posição e o tamanho são seus. Arraste pelo cabeçalho para mover, e puxe
  qualquer um dos quatro lados ou dos quatro cantos para redimensionar. O cursor muda ao chegar
  perto da borda.

Voltar para a grade automática desfaz o arranjo que você montou à mão. O aviso que aparece nessa
troca traz o **Desfazer** junto.

## Escolher o arranjo da grade

O minimapa fica no canto inferior direito. Ele aparece a cada mudança de arranjo e se recolhe num
ícone depois de um instante, voltando quando o cursor chega perto. Clicando nele, você escolhe
entre os arranjos possíveis para a quantidade de painéis abertos: o automático, de uma coluna até
uma coluna por painel, e o de destaque.

## Alinhar à grade

O botão **Alinhar à grade** aparece na barra de comando **só no canvas livre**. Com ele ligado, o
que você move e redimensiona encosta de 40 em 40 pontos. Ao arrastar, só a posição é alinhada; ao
redimensionar, o tamanho também. É uma preferência da sua tela: vale para todos os projetos.

## Selecionar

- **Clique**: seleciona um painel e o traz para a frente.
- **⌘ com clique**: acrescenta à seleção, ou tira dela o que já estava marcado.
- **Arrasto com o botão esquerdo sobre uma área vazia**: desenha um laço que pega tudo o que
  encostar nele, não só o que couber inteiro dentro. A seleção acontece durante o arrasto.
- **Clique numa área vazia**: limpa a seleção.

Arrastar um painel que já está selecionado leva **todos** os selecionados junto.

A cor, a espessura e o brilho do contorno ficam no bloco **Painel selecionado**, na seção
[Aparência](ajustes-aparencia) do editor do projeto. A escolha vale para todos os canvases.

## Fechar

- **O ✕ do cabeçalho** fecha aquele painel.
- **Delete** fecha os painéis selecionados **a partir de dois**. Com um painel só selecionado, a
  tecla não faz nada. Com imagens do canvas selecionadas, ela apaga as imagens em vez dos painéis. E
  ela nunca dispara enquanto você está escrevendo num terminal ou num campo de texto. A tecla é
  configurável em **Configurações → Atalhos**.
- **Por voz**: *"fecha os agentes"*, *"fecha dois navegadores"*, *"fecha o Juno e a Diana"*,
  *"fecha tudo"*. O fechamento por tipo e o *"tudo"* agem só na área de trabalho aberta; por nome,
  alcança painel de qualquer área. Se algum alvo estiver trabalhando, o app devolve a pergunta em
  vez de fechar, e começa pelos que estão parados quando precisa escolher quantos.

## Largura máxima de um painel

Em **Configurações → Interface**, o controle **Largura máxima de um painel** vai de 600 a 4000 px,
com 1500 px de fábrica. Ele limita um painel que está **sozinho** na tela, que fica centralizado;
vários painéis continuam usando a tela toda. Só tem efeito na grade automática, e vale para todos os
projetos. Por voz: *"largura máxima 1500"*.

## Juntar agentes num painel só

Arrastar um agente sobre o cabeçalho de outro põe os dois no mesmo painel, com uma fileira de abas
no alto. A mesma coisa se faz para a área inteira pelo menu da aba, em
[áreas de trabalho](areas-de-trabalho).

## A janela do app

Por voz dá para pôr a janela num formato exato antes de gravar: *"janela em paisagem 1080"*,
*"janela vertical"*, *"janela quadrada"*. Veja [o painel de gravação](painel-gravacao).
