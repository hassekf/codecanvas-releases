---
slug: painel-galeria
titulo: A galeria de imagens
resumo: As imagens deste projeto guardadas em disco: recolocar no canvas, apagar de verdade, e o pedido que gerou cada uma.
area: paineis
nivel: basico
---

Abre pelo `⌘K` (digite "galeria" ou "imagens"). É uma por projeto.

## O que ela guarda

Toda imagem que entrou no canvas deste projeto, colada, arrastada ou gerada. Tirar uma imagem do
canvas não apaga o arquivo: ele continua aqui, e a exclusão definitiva acontece **só** neste painel.

Na miniatura e na legenda:

- **Gerada**: a legenda é o pedido que criou a imagem, e um emblema a marca na miniatura.
- **Colada**: a legenda diz apenas isso.
- Um segundo emblema marca as imagens que estão coladas no canvas neste momento.

## Os gestos da grade

- **Clique numa miniatura**: marca e desmarca. Clicar em várias marca várias.
- **Arrastar a partir de um vão**: desenha um laço e marca tudo o que ele encostar, entre as
  miniaturas visíveis. Um clique no vão limpa a seleção.
- **Arrastar uma miniatura**: leva a imagem para o canvas. Se ela estiver numa seleção de várias,
  o arrasto leva todas as marcadas, uma deslocada da outra.
- **`+` ao passar o mouse**: recoloca a imagem no canvas sem arrastar.

## O menu de cada imagem

- **Adicionar ao canvas**: recoloca a imagem no canvas.
- **Enviar a um contato**: manda a imagem por [recados](painel-recados). O pedido que a gerou vira o
  assunto.
- **Copiar o prompt**: copia o pedido para a área de transferência. Só existe em imagem gerada.
- **Apagar da galeria**: apaga o arquivo, com confirmação.

## O cabeçalho

- **O número ao lado do título**: quantas imagens o projeto tem.
- **Apagar (n)**: apaga as marcadas, com confirmação. Aparece com alguma imagem marcada.
- **Limpar seleção**: desmarca tudo sem apagar nada.
- **Selecionar tudo**, **Atualizar** e **Limpar a galeria toda**, no menu ao lado: o segundo relê a
  pasta do disco; o terceiro apaga todas as imagens do projeto, com confirmação.

## Apagar tira do canvas também

A confirmação muda quando alguma das imagens a apagar está colada no canvas: ela avisa **Apagar do
canvas também?** e nomeia as áreas de trabalho onde a imagem está. Apagar da galeria remove a imagem
do canvas junto, e não há como desfazer.

## Como uma imagem é gerada

Peça à assistente por voz ou a um agente por escrito. Você pode dizer quantas imagens quer (o padrão
é uma), a orientação (quadrado é o padrão, e há paisagem e retrato) e a qualidade daquele pedido.

A geração leva dezenas de segundos: o app responde antes de terminar, cola cada imagem no canvas
quando ela fica pronta e avisa no fim. Pedida a um agente, a imagem nasce perto do painel dele;
pedida por voz, ela nasce em espaço livre no centro da vista.

O pedido e o modelo ficam gravados com o arquivo. É o que a legenda mostra e o que **Copiar o
prompt** entrega.

Isto é diferente do papel de parede do canvas, que tem comandos próprios em
[aparência](aparencia).

### O modelo e a qualidade padrão

Em **Configurações → Conversa**.

- **Modelo de imagem**: o modelo que desenha. A lista é buscada na OpenAI, e **Atualizar** a relê.
- **Qualidade padrão da imagem**: **Econômica**, **Padrão** ou **Alta**. Vale para os pedidos que
  não pedem outra qualidade.

Os dois dependem da sua chave da OpenAI estar cadastrada, na mesma tela. Veja
[configurar a voz](configurar-a-voz) e [quanto custa](quanto-custa).

## As imagens soltas no canvas

Pôr uma imagem no canvas, movê-la, mudar a camada e apagá-la estão em
[imagens no canvas](imagens-no-canvas). Esta página é sobre onde elas ficam guardadas.
