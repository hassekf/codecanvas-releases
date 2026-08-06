---
slug: painel-design
titulo: A superfície de design
resumo: Onde os artboards ficam no canvas, como se navega neles, e como apontar um trecho vira um pedido a um agente.
area: design
nivel: avancado
---

Um arquivo de design é uma pasta com extensão `.design`, que costuma morar no repositório do
projeto. Ele abre **no plano do canvas**: os artboards ficam soltos ali, sem moldura de painel.

- **`⌘K` e design**, **artboard**, **mockup**, **protótipo**, **interface**, **layout**, **figma**,
  **wireframe** ou **desenho**: abre o primeiro `.design` da raiz do projeto. Não havendo nenhum, o
  app abre antes a tela de direção e cria um.
- **`⌘⇧D`, ou o pincel no rodapé**: abre o navegador de design.

Você não edita à mão: não há alças nem inspetor. Os seus gestos sobre um design são mover artboards
e apontar. Quem desenha são os agentes, cada um com o cursor visível na tela.

## O navegador de design

- **No canvas**: os designs em cena. Clicar no nome recolhe e expande a lista de artboards; o número
  ao lado do nome conta os artboards.
- **Uma linha de artboard**: leva a câmera até ele. A linha do artboard que está na seleção viva
  aparece destacada.
- **O lápis**, na linha do design: reabre a direção daquele arquivo, preenchida.
- **A seta**, na linha do design: leva a câmera até o design inteiro.
- **Fechar design**, no menu de contexto da linha: tira o design da tela sem apagar o arquivo.
- **Remover artboard** e **Enviar a um contato**, no menu de contexto de um artboard: apaga o
  artboard do arquivo, ou manda o documento a um contato, com o nome do artboard como assunto.
- **No projeto**: os pacotes `.design` da raiz do workspace que ainda não estão em cena. **Abrir**
  traz um deles para o canvas.
- **Novo design**: abre a tela de direção e cria um arquivo.

Apertar `⌘⇧D` de novo fecha o navegador.

## A direção

A direção é gravada dentro do arquivo e vale para qualquer agente que desenhe ali depois. A tela
pede:

- **Nome**: o nome do arquivo. Só na criação.
- **O pedido**: o brief. É o único campo que a tela trata como necessário.
- **Direção**: um dos estilos oferecidos, ou **O agente decide**.
- **Variância estrutural** e **Densidade**: dois controles deslizantes, de seguro a experimental e de
  esparso a denso.
- **Tema** (**Claro**, **Escuro**, **Ambos**) e **Alvo** (**Desktop**, **Mobile**, **Ambos**).
- **Cor-semente**: uma cor de partida, ou **Auto**.
- **Tipografia**: o par tipográfico. Vazio, o agente escolhe.
- **Regras avançadas**: quatro regras que o agente recebe junto, cada uma com o seu interruptor: a
  ban-list anti-slop, o uso obrigatório dos tokens do arquivo, a auditoria visual antes de entregar,
  e a exigência de que variações mudem de esqueleto.
- **Quem desenha**: **Ninguém por enquanto**, **Um agente novo**, ou um agente aberto no canvas. O
  botão do rodapé muda conforme a escolha.

O que você deixar em branco o agente escolhe, declara e grava no arquivo.

## Apontar

Clique num elemento ou lace uma região: uma caixa nasce colada na seleção.

- **Os verbos** (*mais ousado*, *mais quieto*, *polir*, *mais denso*, *mais leve*, *variar*,
  *alinhar*): cada toque acrescenta a palavra ao seu texto. Reconhecida no envio, ela leva junto uma
  instrução de direção para o agente.
- **O campo de pedido**: `Enter` envia.
- **O nome à direita do campo**: escolhe o agente que recebe. A lista põe na frente os agentes da
  mesma área de trabalho e os acordados. A escolha fica guardada e não se perde ao trocar de seleção
  nem ao enviar.

O agente recebe o seu texto, a descrição do que você selecionou, um recorte em imagem do trecho, um
manifesto com os ids e o caminho do arquivo. Num design ainda vazio, a caixa aparece do mesmo jeito e
o agente é avisado de que não há artboard nenhum.

A seleção continua viva depois do envio: qualquer agente que leia o design encontra nela o referente
de *"esse botão"*.

## Arrastar um artboard para fora

Puxar um artboard para fora da superfície transforma-o num cartão que segue o cursor. Soltando sobre
um painel de agente, ele recebe a citação daquele artboard (o recorte, os ids e o arquivo). Soltando
no vazio, nada acontece e o documento não muda.

## O zoom

O zoom e o arrasto do canvas são os do design: não há uma câmera dentro da outra, e a superfície não
rola por conta própria.

## Quando o arquivo tem problema

- **Arquivo que o app não conseguiu ler**: o pacote fica travado. As ferramentas dos agentes
  respondem com a lista de problemas e **nada é gravado**. Corrigido o arquivo, ele destrava sozinho.
- **Arquivo mudado por fora** (um agente editando o `design.json` direto, um `git checkout`): o app
  recarrega. Havendo conflito com o que estava em memória, o disco vence e o app avisa.

## O que os agentes fazem aqui

Eles leem o documento e a sua seleção, aplicam operações, fotografam o resultado, medem um texto
antes de inseri-lo e trazem uma fonte do Google Fonts para dentro do pacote. Está em
[o agente desenha e gera](o-agente-desenha-e-gera).

Exportar o design para imagem ou para código não existe hoje.
