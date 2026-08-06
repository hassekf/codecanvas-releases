---
slug: o-agente-ve-o-navegador
titulo: O navegador do agente
resumo: O que um agente faz numa página aberta no canvas, e como pedir que ele confira o próprio trabalho.
area: agentes-fazem
nivel: basico
---

Cada agente abre um navegador próprio, como painel do canvas. A imagem da página volta para ele.

## O que pedir

- *"Abre o localhost:3000 e me diz se o cabeçalho ficou alinhado."*
- *"Abre a página, clica em Entrar e me diz o que acontece."*
- *"A tela está em branco. Lê o console e me diz qual é o erro."*
- *"Preenche o campo de e-mail com um valor inválido e vê se a mensagem de erro aparece."*
- *"Rola até o rodapé e confere se os links novos apareceram."*
- *"Me diz qual é o texto do botão de confirmação."*

## O que ele faz na página

- **Abrir um endereço**: aceita `localhost:3000`, `meusite.com:8080` ou uma URL completa.
- **Fotografar**: devolve a imagem da página no estado em que ela está.
- **Clicar**: o alvo é um seletor CSS (`#salvar`, `.btn-primary`) ou o texto visível do elemento
  (`Entrar`). A imagem do resultado vem junto.
- **Digitar num campo**: o alvo é um seletor CSS. Os eventos de input são disparados, então React e
  Vue enxergam o texto. Ele pode apertar Enter no fim, o que resolve busca e login.
- **Rolar**: até o topo, até o fim, até um seletor, ou um número de pixels.
- **Ler o console**: logs, avisos e erros de JavaScript. É a única fonte quando a página aparece em
  branco.
- **Rodar JavaScript na página**: o valor da expressão volta para ele. Serve para ler o texto de um
  elemento, conferir um valor de estado ou checar se um seletor existe.
- **Fechar o navegador**: o painel sai do canvas.

## Um navegador por agente

- O navegador pertence ao agente que o abriu. Nenhum outro agente navega nele.
- Um agente não dirige o navegador que **você** abriu. Esse é o de
  [o painel do navegador](painel-navegador).
- Se ele já tem um navegador aberto, o endereço seguinte vai para o mesmo painel.

## O `open` do terminal vai para o canvas

Quando um agente roda `open` com uma URL ou com um arquivo `.html`, o CanvasCode abre o endereço no
navegador dele, dentro do canvas, e recusa o comando. O agente recebe o motivo e o endereço que foi
aberto.

- Isso vale enquanto o navegador padrão deste projeto for o interno, em
  [ajustes do navegador](ajustes-navegador). Com o externo escolhido, o comando passa direto.
- A escapatória é o marcador `CODECANVAS_EXTERNO=1` na frente do comando: com ele, o endereço abre
  fora do app.
- Um `open .` no Finder, um `open -a` noutro programa e qualquer alvo que não seja uma página não são
  interceptados.

## O que ele não faz

- Não usa o Safari nem o Chrome para conferir o próprio trabalho.
- Não clica em elemento que não existe: ele responde que não achou, em vez de seguir adiante.
