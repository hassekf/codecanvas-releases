---
slug: modulos
titulo: Criar um módulo
resumo: A pasta, o manifesto, as ações que viram ferramentas de voz e o que a página consegue fazer pela ponte do app.
area: modulos
nivel: avancado
---

Um módulo é uma pasta em `Application Support/codeCanvas/modulos/<id>/`, e o nome da pasta é o id do
módulo. Duas peças são obrigatórias: `modulo.json` e `index.html`. Como ele se comporta depois de
pronto está em [o painel de um módulo](painel-modulos).

Não há instalador nem registro: o app vigia a pasta. Criar faz o módulo aparecer, corrigir o traz de
volta, apagar o tira do app.

## Pedir a um agente

Peça a um agente do canvas: *"cria um módulo que mostra o saldo da minha conta do banco X"*. Ele
carimba a pasta com o esqueleto, edita, abre o painel, tira uma foto dele, lê o console e corrige.

O esqueleto vem com o manifesto preenchido, uma página que já usa a ponte, um script de exemplo já
declarado como ação, e o arquivo `CONTRATO.md` com a referência completa na versão deste app.

O id sai do nome, em minúsculas, sem acentos e sem espaços. Um nome que colida com um painel nativo
do app é recusado, e um id que já exista também.

## O manifesto

- **`formato`**: a versão do contrato. Obrigatório, e hoje é `1`. Um formato maior do que o app
  conhece é recusado inteiro, com o motivo.
- **`nome`**: obrigatório. É o nome no painel, no `⌘K` e na voz.
- **`descricao`**: a linha embaixo do nome no catálogo e na barra do painel.
- **`icone`**: um símbolo do SF Symbols.
- **`palavras`**: sinônimos que a busca do `⌘K` aceita.
- **`varios`**: `true` permite mais de um painel deste módulo por canvas.
- **`usaContexto`**: documenta que o conteúdo varia por projeto. Não muda o comportamento do app.
- **`recarregarACada`**: recarrega a página sozinha a cada N segundos, no mínimo 5.
- **`semMoldura`**: `true` faz o painel solto esconder cabeçalho e borda.
- **`acoes`**: as ferramentas que o módulo dá à Nina e aos agentes.

## As ações

Cada ação tem um **`nome`** (minúsculas, números e `_`), uma **`descricao`** e um **`script`** da
própria pasta. Chamada, o app roda o script e devolve a saída padrão a quem chamou; a Nina responde
falando em cima dela.

A `descricao` é o campo que decide quando a ação é chamada: escreva o que ela faz, o que devolve e em
que pedido usar. Vaga, ela é chamada na hora errada, ou nunca.

A saída precisa ser curta e legível. Erro vai para a saída de erro, com código de saída diferente de
zero, e é isso que o app repassa como falha.

A Nina recebe as ações na abertura da conversa: ligar ou desligar o interruptor de um módulo vale a
partir da conversa seguinte. Os dois interruptores estão em
[o painel de um módulo](painel-modulos).

## O que a página consegue fazer

A página recebe uma ponte para o app: requisição sem restrição de origem, rodar um script da pasta,
saber em que projeto está, adotar o tema, guardar dados e notificar você. Está em
[as capacidades de um módulo](modulos-capacidades).

## Por onde seguir

- O conceito: [o que é um módulo](modulos-o-que-e).
- O painel na tela e a lista em Configurações: [o painel de um módulo](painel-modulos).
