---
slug: painel-terminal
titulo: O painel de terminal
resumo: Um shell na pasta do projeto, dentro do canvas: como abrir, o que os gestos fazem, e de onde vêm a fonte e o nome.
area: paineis
nivel: basico
---

Um shell do sistema rodando na pasta do projeto deste canvas, sem agente nenhum em cima dele.

## Abrir e fechar

- **`⌘K`, digitando "terminal"**: abre um painel novo. Cada chamada abre mais um, ao contrário do
  [painel do Git](painel-git) e do [painel do elenco](painel-elenco), que são um por canvas.
- **`⌘T`**: o mesmo, sem passar pela [busca](busca-e-comandos). A tecla é trocável em
  Configurações → Atalhos.
- **Fechar o painel encerra o processo.** Trocar de canvas não: o shell continua rodando fora de
  vista, e o painel volta com o que ele imprimiu enquanto você estava noutro projeto.

## O nome do painel

- **Dois cliques no título**: abre o campo de edição. Enter confirma, Esc desiste, e clicar fora
  também confirma.
- **O terminal é o único painel com nome editável.** O agente já tem nome próprio, e os demais
  derivam o título do que mostram.
- **O nome é endereço.** É por ele que a [busca](busca-e-comandos), a Nina e os agentes encontram o
  painel: um terminal chamado "deploy" passa a responder por "deploy" nos três.

## Gestos dentro do terminal

- **Clique num caminho impresso**: o app procura o arquivo no disco e abre onde ele se lê melhor,
  um [painel de arquivo](painel-arquivo) para texto, o navegador para uma página, o Finder para o
  resto. Caminhos relativos contam a partir da pasta em que este terminal está. Não encontrando
  nada, o app avisa em vez de abrir uma janela vazia.
- **Clique num endereço da web**: abre num [painel de navegador](painel-navegador), ou no navegador
  do sistema se este canvas estiver configurado para o externo, na aba **Agentes** dos
  [ajustes do projeto](ajustes-projeto).
- **Arrastar arquivos do Finder para dentro**: escreve os caminhos, escapados, na linha de comando.
  Nada é executado, e nenhum agente é acionado.

## A letra

- **O zoom do canvas muda o tamanho da fonte**, e o texto continua nítido em qualquer zoom.
- **Fonte e tamanho de partida**: Configurações → Terminal. Só fontes monoespaçadas são oferecidas,
  e a escolha vale para todos os terminais e agentes do app, inclusive os fora de vista.

## Comandos que não terminam

Um agente que roda um servidor de desenvolvimento, um observador de arquivos ou qualquer comando que
não retorna fica preso nele. O app desvia esses comandos para um painel de terminal próprio, visível
no canvas, e avisa o agente do desvio. Comandos que terminam passam direto.

Isso é o ajuste **Dev servers em painel próprio**, em Configurações → Agentes. Desligado, o agente
roda tudo dentro de si, e um servidor prende a conversa dele sem aparecer em lugar nenhum. Mais em
[falar com eles](falar-com-eles).
