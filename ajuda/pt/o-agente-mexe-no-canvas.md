---
slug: o-agente-mexe-no-canvas
titulo: O agente mexe no canvas
resumo: Abrir painéis, mostrar arquivos, tocar mídia, escrever o assunto do painel e disparar anúncios.
area: agentes-fazem
nivel: basico
---

## O que pedir

- *"Escreve o plano num arquivo e abre aqui na tela."*
- *"Faz o relatório e me mostra, em vez de colar tudo no terminal."*
- *"Abre o painel do Git aqui do lado enquanto você trabalha."*
- *"Acha um vídeo sobre concorrência em Swift e põe pra rodar."*
- *"Bota uma playlist de foco, só o áudio."*

## Mostrar um arquivo

Um agente abre qualquer arquivo do projeto num painel. Markdown é renderizado e imagens aparecem. O
caminho é relativo à pasta do projeto. Veja [o painel do arquivo](painel-arquivo).

## Abrir painéis

Um agente abre os painéis do canvas pelo tipo: terminal, navegador, Git, elenco, tarefas, notas,
recados, mídia, galeria, gravação, webcam, uso, desempenho, Jira, iniciativas, design e os módulos
que você criou.

- **Um agente não abre outro agente.** O tipo não aparece na lista dele, e um pedido nesse tipo é
  recusado. Quem cria agente é você, ou um agente que você mandou chamar colegas, por outro caminho
  ([o agente chama colegas](o-agente-chama-colegas)).
- Ele não fecha nem reposiciona os painéis que você abriu.

## Tocar mídia

Um agente põe vídeo ou música no [painel de mídia](painel-midia), que abre se ainda não estiver
aberto. Duas formas:

- **Um endereço**: ele pesquisa, escolhe e manda o link direto do vídeo, da playlist ou da música.
- **Um termo de busca**: a lista de resultados aparece na tela e a escolha é sua.

Ele também encolhe o painel numa cápsula, mantendo o som, e o traz de volta ao tamanho normal.

## O assunto do painel

O agente escreve o que está fazendo: um assunto curto, um contexto de duas a quatro frases, e o que
ele espera de você, quando espera.

- O assunto vira a linha de contexto do painel dele. O contexto e a pendência aparecem no verso do
  painel, e a Nina os lê em voz alta quando você pergunta como estão todos. Veja
  [saber o que fazem](saber-o-que-fazem).
- **O texto que você fixou à mão tem precedência.** Enquanto ele existir, a linha do painel é a sua,
  e o que o agente anotar não a substitui.
- Trocar de assunto encerra o anterior e o registra como uma entrega, com o contexto daquele momento.
  Isso depende do histórico de entregas estar ligado em [ajustes dos agentes](ajustes-agentes).
- O assunto escrito pelo agente não altera o estado dele (trabalhando, esperando, parado, caído).

## Disparar um anúncio

Os anúncios são os alertas que você escreveu em [anúncios](ajustes-anuncios), com nome, regra, estilo
e texto. O agente dispara um deles pelo nome e preenche os marcadores que faltam, como o número da
versão.

- Ele não cria anúncio, não edita o texto e não dispara nome que não esteja na sua lista.
- **O mesmo anúncio disparado por vários agentes aparece uma vez.** Se ele já está na tela ou na
  fila, os disparos seguintes são ignorados.
- Um anúncio não interrompe: com o microfone aberto, com a Nina em conversa ou em modo reunião, ele
  entra na fila e aparece quando você estiver livre. Um de cada vez.
