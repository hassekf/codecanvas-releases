---
slug: design-no-canvas
titulo: Design no canvas
resumo: A superfície onde os agentes desenham telas e você dirige apontando, com o arquivo versionado no projeto.
area: design
nivel: basico
---

O CanvasCode tem uma superfície de design própria. **Os agentes desenham, e você dirige**: clica num
elemento ou laça uma região e pede dali. Cada agente que está desenhando aparece com um cursor
próprio na tela.

Você não edita à mão. Não há alças, inspetor nem texto editável no painel, e os seus gestos sobre um
design são dois: mover artboards e apontar.

## O arquivo

Um design é uma pasta com extensão `.design`, que o Finder mostra como se fosse um arquivo. Dentro
dela ficam o documento e as imagens e ícones que ele usa.

- **Ele costuma morar no repositório do projeto**, versionado com o código. O desenho entra no
  histórico, viaja para quem clonar o projeto e pode ser lido por qualquer agente como especificação.
- **Um design aberto não é um painel**: ele abre no plano do canvas, com os artboards soltos ali.
- **Cada tela, variação ou versão mobile é um artboard** dentro do mesmo arquivo. Um arquivo novo só
  nasce quando o assunto muda.

## O que dá para pedir

- **Telas e variações**: *"desenha três variações da tela de login: uma clássica, uma com foto de
  fundo, uma minimalista"*. Um pedido com muitas telas vira um agente por tela, desenhando ao mesmo
  tempo.
- **Ajustes apontados**: selecione um botão e peça *"deixa maior e com mais respiro embaixo"*.
- **Fluxos inteiros**: *"desenha o fluxo de cadastro, quatro telas"*.
- **Tipografia de verdade**: o agente traz uma família do Google Fonts para dentro do pacote, com os
  pesos que usar. Dali em diante a fonte viaja com o arquivo e funciona sem internet.
- **Ícones**: ele usa um catálogo de cerca de dois mil ícones, e o que ele usar é gravado dentro do
  pacote.
- **Seguir referências**: as imagens que você colou no canvas ficam disponíveis para ele. Veja
  [imagens no canvas](imagens-no-canvas).

O que o agente faz enquanto desenha, e o que ele mede e confere antes de entregar, está em
[o agente desenha e gera](o-agente-desenha-e-gera).

## Os tokens

O arquivo guarda o próprio vocabulário de cores e medidas, e é com ele que todos os agentes pintam.
Trocar um token muda tudo o que o usa, em todos os artboards, de uma vez. Um agente que precisa de
uma cor nova declara um token em vez de escrever a cor solta.

## A direção

Todo design tem uma direção escrita dentro do arquivo: o pedido, o estilo, o tom, a paleta, o par de
fontes e as regras que o agente tem de respeitar. É ela que faz dois agentes desenharem a mesma
coisa em vez de dois produtos diferentes. Veja [a direção do design](design-direcao).

## O que ele não é

- **Não é um editor tipo Figma.** Isso é recorte de produto: quem desenha são os agentes.
- **Não exporta para imagem nem para código** hoje.
- **Não é o painel de imagens.** Uma imagem gerada é outra coisa, e fica na
  [galeria](painel-galeria).

Para codificar a partir do desenho, um agente lê o próprio arquivo do design: ele é a especificação,
e não precisa de exportação.

## Por onde começar

1. `⌘⇧D`, ou o pincel no rodapé, abre o navegador de design.
2. **Novo design** pede a direção e cria o arquivo.
3. Escolha quem desenha, e peça a primeira tela.

A tela e os gestos estão em [o painel de design](painel-design).
