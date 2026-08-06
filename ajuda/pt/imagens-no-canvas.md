---
slug: imagens-no-canvas
titulo: Imagens no canvas
resumo: Colar e arrastar imagens para o espaço do canvas, movê-las, mudar a camada e apagá-las.
area: canvas
nivel: basico
---

Uma imagem colada no canvas não é um painel: ela não entra no arranjo automático, não tem cabeçalho e
fica onde você a deixou, em qualquer um dos dois modos da mesa.

## Pôr uma imagem no canvas

- **`⌘V`**: cola a imagem da área de transferência no centro da vista.
- **Arrastar um arquivo de imagem** do Finder para um vão do canvas: o mesmo efeito.
- **Arrastar uma miniatura da galeria**, ou o `+` que aparece sobre ela: recoloca uma imagem que já
  está guardada. Veja [a galeria](painel-galeria).
- **Um agente**, ao gerar uma imagem que você pediu: ela nasce em espaço livre perto do painel dele.
  Veja [o agente desenha e gera](o-agente-desenha-e-gera).

O arquivo é copiado para dentro do app. A imagem não aponta para a pasta de origem, e não é gravada
dentro da pasta do projeto: apagar o original depois não apaga a imagem do canvas.

## Mexer numa imagem

- **Arrastar**: move. A imagem inteira é a alça.
- **Clique**: seleciona e abre a barra da imagem, com legenda, opacidade, **Para a frente**, **Para
  trás** e **Apagar**.
- **Para a frente** põe a imagem acima dos painéis; **Para trás** a devolve à camada de baixo.
- **Apagar**, nessa barra, tira a imagem do canvas e a mantém na galeria.
- **Delete**, com imagens selecionadas: apaga as imagens em vez dos painéis selecionados.

## O que ela não faz

- **Não entra no arranjo automático.** Ao organizar o canvas, as imagens só saem de baixo dos
  painéis, para a vaga livre mais próxima, com o tamanho que tinham. Veja
  [organizar sozinho](organizar-sozinho).
- **A roda do mouse sobre ela é da câmera**, e não da imagem: ela não é painel.
- **Não é o papel de parede.** O fundo do canvas se escolhe em [aparência](aparencia).

## Levar imagens para outro lugar

- **Para outra área de trabalho**: as imagens selecionadas vão junto quando você arrasta os painéis
  selecionados até a aba de destino. Veja [áreas de trabalho](areas-de-trabalho).
- **Para um agente**: soltar um arquivo **sobre o painel de um agente** cola o caminho no prompt
  dele, sem enviar, em vez de virar imagem no canvas.
- **Para outra pessoa**: pelo menu da imagem na galeria, em **Enviar a um contato**. Veja
  [os recados](painel-recados).

## O que os agentes veem

As imagens do canvas ficam disponíveis para os agentes deste projeto, que listam e abrem cada uma
pelo caminho, e enxergam o conteúdo delas. Serve para print de erro, foto de tela e rascunho de papel
fotografado, sem você descrever em palavras o que está na figura.

## Onde elas ficam guardadas

Toda imagem que entra no canvas vai para a galeria do projeto, e é lá que ela se apaga de verdade.
Veja [a galeria](painel-galeria) e [onde ficam meus dados](onde-ficam-meus-dados).
