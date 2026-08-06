---
slug: o-agente-desenha-e-gera
titulo: O agente desenha e gera imagens
resumo: Pedir telas na superfície de design, apontar o que mudar, gerar imagens no canvas e usar as referências que você colou.
area: agentes-fazem
nivel: avancado
---

## O que pedir

- *"Desenha três variações da tela de login: uma clássica, uma com foto de fundo, uma minimalista."*
- *"Deixa esse botão maior e com mais respiro embaixo."*
- *"Desenha o fluxo de cadastro, quatro telas."*
- *"Traz uma fonte melhor para os títulos."*
- *"Gera um mascote de raposa, flat, fundo branco."*
- *"Olha as referências que eu colei aqui no canvas e segue esse clima."*

O que a superfície de design é e o que ela guarda está em [o painel de design](painel-design).

## Desenhar

O agente lê o arquivo de design, edita e fotografa o resultado. Você vê cada mudança aparecer no
painel enquanto ela acontece.

- Ele cria e altera artboards, frames, retângulos, elipses, textos, traçados, imagens e ícones, com
  layout, preenchimento, contorno, canto arredondado, sombra e desfoque.
- Ele define os **tokens** do arquivo, o vocabulário de cores e medidas com que todos os agentes
  pintam.
- **Uma tela nova, uma variação ou a versão mobile de algo entram como artboard no arquivo aberto.**
  Um pacote novo só nasce quando o assunto muda ou quando você pede separado.
- **Você não desenha à mão.** Não há alças, inspetor nem texto editável no painel. Os seus gestos
  sobre o design são mover telas e apontar.

## Apontar

Clique num elemento do design, ou lace uma região, e o pedido passa a ter referente.

- A seleção viaja junto da mensagem: um recorte em imagem do que você apontou, mais os identificadores
  e as medidas daquele trecho.
- O agente que recebe o apontamento é escolhido no próprio painel de design, e a escolha fica gravada
  entre um pedido e o seguinte.
- **Sete palavras carregam instrução de direção quando aparecem no que você escreve**: `mais ousado`,
  `mais quieto`, `polir`, `mais denso`, `mais leve`, `variar` e `alinhar`. Elas valem para a região
  apontada.

## Várias telas de uma vez

Um pedido com muitas telas ou muitas variações vira um agente por tela, cada um restrito ao próprio
artboard, trabalhando ao mesmo tempo. Quem divide é o agente que recebeu o pedido, pelo mesmo caminho
de [o agente chama colegas](o-agente-chama-colegas).

## A direção do arquivo

Todo design tem uma direção escrita: o estilo, o resumo do produto, o tom, a coisa memorável da tela,
a paleta e o par de fontes. Ela é preenchida quando o design nasce, e você a reabre e edita depois.

- Um agente não muda estilo, paleta nem fontes do arquivo sem você pedir.
- Um arquivo sem direção não recebe o primeiro elemento: o agente é mandado escrevê-la antes.

## Tipografia

- **Medir**: o agente mede um texto com a fonte real do arquivo antes de inserir, e recebe largura e
  altura em pixels. Para parágrafo, ele passa a largura máxima e recebe a altura com as quebras
  reais. A medida é do texto puro, sem o espaçamento interno da caixa.
- **Trazer uma família do Google Fonts** para dentro do pacote, com os pesos que ele for usar. O
  download acontece em segundo plano e os textos trocam de fonte quando ele termina. Dali em diante a
  fonte viaja com o arquivo e funciona sem rede.

## Gerar imagens

A imagem nasce no canvas, em espaço livre ao lado do painel de quem pediu.

- O agente escolhe a quantidade e a orientação: paisagem, retrato ou quadrado.
- O modelo e a qualidade vêm das suas Configurações. Ele pode pedir outra qualidade só naquela
  chamada, entre baixa, média e alta.
- O teto do modelo vence a quantidade pedida: alguns geram uma imagem por vez.
- Toda imagem gerada fica na [galeria](painel-galeria), com o pedido que a criou.
- Isso não é papel de parede. O fundo da tela se muda em [aparência](aparencia).
- Gerar imagem usa a sua chave da OpenAI, a mesma da voz. Sem ela, o agente recebe o aviso de que a
  chave falta.

## As referências que você colou

As imagens que você cola ou arrasta para o canvas ficam disponíveis para os agentes. Um agente lista
essas imagens e abre cada uma pelo caminho, e ele enxerga o conteúdo delas.

Serve para print de erro, foto de tela e rascunho de papel fotografado, sem você descrever em
palavras o que está na figura.
