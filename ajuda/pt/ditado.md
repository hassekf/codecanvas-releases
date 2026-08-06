---
slug: ditado
titulo: Ditado
resumo: ⌥D e falar: para onde o texto vai, o que vira símbolo, os dois motores e o ditado longo.
area: nina
nivel: basico
---

**⌥D** dita para um agente. A tecla se troca em **Configurações → Atalhos**, na linha "Ditar", e o
motor de transcrição se escolhe em **Configurações → Voz**.

O texto chega ao agente palavra por palavra, sem nenhum modelo reescrevendo o que você disse.

## A tecla

- **Segurar e soltar**: enquanto a tecla estiver pressionada o app escuta; soltar envia.
- **Tocar e soltar**: a escuta fica travada e você fala à vontade. A janelinha passa a dizer "toque
  de novo para enviar", e é esse toque que envia.
- **Esc**: cancela. O texto é descartado e não chega a agente nenhum.

Com a escuta travada, um minuto de silêncio pausa o ditado. O que você falou fica guardado num aviso
com três saídas: **Continuar falando**, **Enviar** e **Descartar**. Sem um agente escolhido, o aviso
pede que você clique no painel de quem vai receber, e o envio fica indisponível até lá.

## Para onde o texto vai

As regras são fixas, sem modelo nenhum decidindo:

- **"Peça pro Marshall extraia o guard clause pro topo"**: vai literal para o Marshall. Ele reconhece
  várias formas de endereçar ("peça pro", "pede pro", "manda pro", "fala pro", "diz pro", "ei") e
  tira o nome e os conectores do começo do texto.
- **"Foco no Marshall"**: destaca o painel dele, sem enviar texto.
- **Qualquer outra frase**: vai para o agente selecionado. Com um único agente no canvas, vai para
  ele.
- **Com [a conversa escrita](a-nina-por-texto) aberta**: cai no campo dela.

O nome é reconhecido ignorando acento e maiúscula. A janelinha do ditado mostra o destino ao lado do
texto, ou "sem destino" quando não há para quem mandar. **Um arquivo selecionado no canvas viaja junto
com o texto**, como referência na frente do que você ditou, e a janelinha marca isso ao lado do nome
do destinatário.

- **Fio do ditado** (Configurações → Interface): liga o fio que sai da barra do ditado até o painel
  que vai receber o texto. Desligado, o destino continua escrito ao lado da barra.

## A pontuação ditada

Quatro palavras viram símbolo quando estão entre dois pedaços que parecem identificador:

- **"underline"** e **"sublinhado"** viram `_`.
- **"barra"** vira `/`. "Src barra components" vira `src/components`.
- **"hífen"** vira `-`.
- **"ponto"** vira `.` apenas antes de uma extensão de arquivo conhecida. "Index ponto tsx" vira
  `index.tsx`; "até que ponto é viável" fica como você falou.

A conversão não acontece quando um dos lados é palavra comum, como em "na nossa barra aqui embaixo".
Fora isso, o ditado não mexe na sua pontuação nem corrige o seu texto.

## Os dois motores

Em Configurações → Voz → Modelo de transcrição.

- **Sistema (Apple)**: já vem no macOS e mostra o texto enquanto você fala. É o padrão.
- **Parakeet v3**: baixa cerca de 600 MB, uma vez, pelo botão do próprio bloco, e roda no seu Mac
  sem internet. Ele transcreve quando você **solta** a tecla: durante a fala a janelinha mostra
  "ditando…", e o texto chega no fim.

O ditado acompanha o idioma escolhido para o app. Quem continua entendendo só português são as ordens
faladas do [modo comando](o-modo-comando).

## Ditado longo

Em **Configurações → Diagnóstico**, quatro interruptores que valem só para o Parakeet e só para falas
de mais de uns quinze segundos. Todos nascem ligados.

- **Evitar troca de idioma**: impede o texto de escorregar para o inglês no meio do português.
- **Recuperar trechos perdidos**: reconstrói palavras comidas na emenda entre as janelas do ditado.
- **Cortar a fala longa em pedaços**: divide o áudio nos silêncios e transcreve cada pedaço à parte.
  Deixa a fala longa um pouco mais lenta.
- **Ancorar o idioma em cada pedaço**: põe uma palavra do idioma na frente de cada pedaço e a remove
  do texto final.

## Mandar de novo para outro agente

```
"aquilo da migração, joga pro Hermes"
"mandei errado, reenvia o último pro Apolo"
```

O app procura no histórico o que você já ditou e o entrega ao outro agente, sem você repetir a frase.
É um pedido de voz, então vale por ⌥C ou por ⌥X.

## Limites

- Ditado e conversa disputam o mesmo microfone: abrir a conversa com a tecla do ditado pressionada é
  recusado, com aviso.
- Em [modo reunião](agenda-e-reunioes) o ditado não abre o microfone, e o app mostra uma notificação
  dizendo que ele está com a chamada.
