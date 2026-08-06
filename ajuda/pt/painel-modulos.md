---
slug: painel-modulos
titulo: O painel de um módulo
resumo: Como abrir um painel que você mesmo escreveu, o que a barra dele faz, e os dois interruptores de cada módulo.
area: modulos
nivel: avancado
---

Um módulo é um painel escrito por você (ou por um agente seu) e instalado numa pasta do seu Mac.
Para escrever um, veja [módulos](modulos).

Abra com `⌘K` e o nome do módulo, ou as palavras de busca que o manifesto dele declarou. Por voz, o
módulo é aberto pelo nome do manifesto.

Por padrão é um painel por canvas: pedir o mesmo módulo de novo seleciona o painel que já existe. Um
módulo pode declarar que aceita vários.

O módulo fica disponível em todos os projetos. Cada abertura cria um painel daquele canvas, e a
página sabe em que projeto está: o mesmo módulo pode mostrar coisas diferentes em cada um.

## A barra do painel

- **A linha à esquerda**: a descrição do manifesto.
- **Recarregar o módulo**: recarrega a página.
- **Revelar a pasta no Finder**: abre a pasta do módulo.

Um módulo pode declarar que vive fora da grade. Nesse caso o cabeçalho, a borda e esta barra somem
enquanto o painel está solto, e o conteúdo preenche o painel inteiro; um clique revela os controles
de volta, e devolvê-lo à grade traz a moldura.

Um módulo pode declarar também um intervalo de recarga (no mínimo cinco segundos), e aí a página se
recarrega sozinha.

## Enquanto você escreve o módulo

O app vigia a pasta: salvar um arquivo recarrega os painéis daquele módulo, sem reiniciar nada e sem
reabrir o painel. Painéis de outros módulos não são tocados.

O painel também fala quando algo está errado, em vez de ficar em branco:

- **Este módulo está com problema**: o manifesto ou a pasta não passaram na validação. O texto diz o
  quê, e o botão revela a pasta no Finder.
- **Este módulo não existe mais**: a pasta sumiu do disco. Se ela voltar, o painel volta junto.
- **Este módulo está desativado**: o módulo está inteiro, mas desligado nas Configurações.

Um erro de JavaScript da página não derruba o app: ele fica no console daquela página, e os agentes
leem esse console.

## Configurações → Módulos

A tela lista os módulos válidos e os que não passaram na validação, estes com o motivo escrito e um
botão **Revelar**.

- **O interruptor de cada módulo**: desligado, o módulo some da busca, da voz e do alcance dos
  agentes. Um painel dele que esteja aberto diz que o módulo está desativado, em vez de sumir da sua
  frente.
- **Ferramentas para a Nina**: só aparece em módulo ativo e com ações. Desligado, a assistente volta
  a só abrir e fechar o painel, e as ações saem do vocabulário dela na próxima conversa.
- **Revelar a pasta de módulos no Finder**, no rodapé: abre a pasta onde todos moram.

Módulo novo nasce ativo e com as ações disponíveis.
