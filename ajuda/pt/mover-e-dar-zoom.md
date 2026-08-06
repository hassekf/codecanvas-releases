---
slug: mover-e-dar-zoom
titulo: Mover e dar zoom
resumo: Os gestos que movem a câmera do canvas, os limites do zoom, e o que muda na tela quando você se afasta.
area: canvas
nivel: basico
---

## Andar pelo canvas

- **Rolagem do trackpad sobre uma área vazia**: desloca a câmera. Sobre um painel, a rolagem é do
  painel.
- **Arrasto com o botão direito sobre uma área vazia**: desloca a câmera. Sobre um painel, o botão
  direito abre o menu daquele painel.

A gaveta de arquivos, o navegador de design, a barra de frentes e a
[estante](minimizar-e-a-estante) consomem a rolagem como se fossem painéis: sobre eles, a roda rola
a lista.

A câmera é de cada [área de trabalho](areas-de-trabalho). Cada aba guarda a posição e o zoom em que
você a deixou.

## Aproximar e afastar

- **Pinça no trackpad**: aproxima e afasta, inclusive com o cursor sobre um painel.
- **⌘ com rolagem**: o mesmo, inclusive sobre um painel.
- **Roda do mouse sobre uma área vazia**: aproxima e afasta sem modificador. Sobre um painel, a roda
  é do painel. Uma imagem solta no canvas não é painel, e sobre ela a roda continua sendo da câmera.
- **Botões − e +**, no canto superior direito: cada clique muda o zoom num passo fixo, ancorado no
  centro da vista.

Nos gestos, o ponto que está sob o cursor fica parado. O zoom vai de 15% a 300%.

## Devolver a câmera ao lugar

- **Clique na porcentagem**, entre o − e o +: põe o zoom em 100% e desfaz o deslocamento. A grade se
  aperta para não cobrir os painéis soltos, e as imagens do canvas saem de baixo do que as escondia.
- **Clique da roda do mouse**: faz o mesmo. Os botões laterais do mouse não.

## O que deixa de ser desenhado à distância

No canvas livre, abaixo de 40% de zoom, os navegadores, os módulos e os designs viram um retângulo
com ícone e nome. Acima disso, no máximo dez deles ficam desenhados ao mesmo tempo, começando pelos
mais próximos do centro da vista. Os painéis de mídia e de webcam nunca entram nessa conta, e os
agentes e terminais também não: eles desenham em qualquer zoom. Na grade automática, todos ficam
desenhados.

Nada é encerrado nesse momento. O agente que estava trabalhando continua trabalhando, a página do
navegador continua carregada, e o painel volta a desenhar assim que você se aproxima.


## A grade do fundo

A grade quadriculada só é desenhada no canvas livre. O espaçamento dela é de 40 pontos e dobra
conforme você se afasta. Os dois modos da mesa estão em [os painéis e a mesa](os-paineis-e-a-mesa).

## Achar um painel que saiu da vista

- **⌘⇧E**: abre a [estante](minimizar-e-a-estante), com tudo o que está aberto neste projeto.
- **⌘K**: acha um painel pelo nome, em qualquer área de trabalho. Veja
  [busca e comandos](busca-e-comandos).
- **⌥O**: arruma os painéis sem sobreposição. Veja [organizar sozinho](organizar-sozinho).

Por voz, *"me leva no Hermes"* leva a câmera até ele, trocando de projeto e de área antes se ele
estiver noutro lugar.

## As teclas dos projetos

Em **Configurações → Atalhos**, no grupo do canvas, o bloco **Ir para o projeto 1…9**. A posição é a
do cartão na tela inicial, descrita em [vários canvases](varios-canvases).

O seletor tem dois modos:

- **Um modificador para as nove posições**: ⌘ de fábrica, o que dá ⌘1, ⌘2, ⌘3 e assim por diante.
  Sem nenhum modificador marcado, as nove posições ficam sem atalho.
- **Uma tecla por posição**: cada posição recebe a combinação que você gravar, e a que ficar em
  branco não tem atalho.

O aviso no alto da tela de atalhos lista as teclas pedidas por duas ações ao mesmo tempo, e inclui
estas nove.
