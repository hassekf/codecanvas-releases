---
slug: painel-arquivo
titulo: O painel de arquivo
resumo: Ler um arquivo do projeto num painel, editá-lo quando o lápis aparece, e o que acontece quando o disco muda por baixo.
area: paineis
nivel: basico
---

Um arquivo do projeto aberto num painel do canvas.

## Abrir

- **Pela gaveta de arquivos**, no rodapé: dois cliques num arquivo o abrem.
- **Pelo `⌘K`**, digitando o nome do arquivo.
- **Por um agente**, quando ele quer te mostrar alguma coisa.
- **Por voz**: *"me mostra o README"*.

Um arquivo já aberto não gera um segundo painel: o que existe é trazido para a frente.

## A gaveta de arquivos

- **O campo no topo** filtra a árvore pelo nome.
- **Um clique** num arquivo o anexa ao próximo prompt que você mandar. A faixa embaixo da árvore diz
  qual está anexado, e o **×** dela desfaz o anexo.
- **Dois cliques** abrem o arquivo num painel.
- **O olho no topo** mostra e esconde os arquivos que começam com ponto. A escolha vale para todos
  os projetos, e a árvore se refaz sozinha ao virá-la.
- **Clique direito**: **Abrir para ler**, **Copiar caminho**, **Copiar caminho relativo**, **Mandar
  para…** (a um agente deste canvas, sem passar pela área de transferência) e **Revelar no Finder**.

## O que o painel mostra

- **Markdown** vem renderizado. O botão do cabeçalho alterna entre **Ver o fonte** e **Ver
  renderizado**, e só existe em arquivos de Markdown.
- **Código** vem com numeração de linha e realce de sintaxe.
- **Imagem** aparece ajustada ao painel. Clicar alterna entre ajustada e tamanho real, e o rodapé
  mostra as dimensões em pixels. O clique direito oferece **Copiar imagem** (o conteúdo, não o
  caminho), **Copiar caminho** e **Revelar no Finder**.
- **Vídeo** toca com os controles do sistema.
- **Arquivo binário** é declarado como tal, com o tamanho.
- **Arquivo que não existe mais** diz isso no lugar do conteúdo.

O painel recarrega sozinho quando o arquivo muda no disco, inclusive imagens regeradas por um
agente.

## Os botões do cabeçalho

- **Editar** (o lápis): entra no modo de edição. Aparece só em texto e Markdown, com o arquivo
  gravável, inteiro e de até 1 MB.
- **Copiar o caminho completo**: põe o caminho absoluto na área de transferência.
- **Revelar no Finder**: seleciona o arquivo no Finder.

O clique direito, tanto no cabeçalho quanto no conteúdo, traz **Copiar o caminho completo**,
**Enviar para um agente** e **Enviar a um contato**. Os agentes deste canvas aparecem direto; os dos
outros projetos ficam em submenus, e mandar para lá não troca o seu canvas.

## Editar

- **Salvar** (`⌘S` ou o botão): grava no disco. Não há salvamento automático. A tecla vale para o
  painel selecionado, o que decide qual arquivo é gravado quando há dois em edição.
- **Reverter ao salvo**: devolve o texto ao que está no disco, sem sair da edição. Indisponível
  quando não há mudança pendente.
- **Sair da edição**: com mudança pendente, pergunta antes de descartar, com **Descartar** e
  **Continuar editando**.
- **O ponto ao lado do nome do arquivo** indica que existe mudança não salva.

Um arquivo cortado por tamanho não pode ser editado, porque gravá-lo de volta gravaria o corte. A
leitura corta em 4 MB, com o aviso no fim do texto.

## Quando o disco muda por baixo da sua edição

Uma faixa aparece assim que o arquivo muda no disco enquanto há edição não salva, dizendo o nome de
quem mexeu quando ele é identificável. Ela **impede o salvamento** até você escolher:

- **Recarregar**: descarta o que você escreveu e traz o que está no disco.
- **Salvar por cima**: grava o seu texto sobre a mudança do disco.

Fora do modo de edição, o painel apenas acompanha o disco, sem faixa nenhuma.

Salvar registra você como autor daquele arquivo, e o [painel do Git](painel-git) passa a marcar
disputa entre você e um agente.
