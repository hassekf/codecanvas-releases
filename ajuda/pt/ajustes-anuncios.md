---
slug: ajustes-anuncios
titulo: Anúncios
resumo: Alertas visuais que você desenha e os agentes deste projeto disparam ao cumprir uma regra sua: os campos, os marcadores e quando eles aparecem na tela.
area: projeto
nivel: basico
---

Nos [ajustes do projeto](ajustes-projeto), seção **Anúncios**. A lista é de cada canvas.

## A lista

Cada linha mostra o ícone, o nome, o estilo e a regra de disparo, e traz:

- **O interruptor**: ativa e desativa. Desativado, o anúncio continua guardado e apenas para de
  disparar.
- **O lápis**: abre o anúncio no editor abaixo da lista. Clicar na linha faz o mesmo.
- **A lixeira**: exclui o anúncio.
- **Novo anúncio**: cria um anúncio vazio e o abre no editor.

## O editor

- **Nome — como o agente o chama**: a chave do anúncio. O agente dispara dizendo este nome, e um
  nome que ele não reconheça não dispara nada.
- **Quando disparar — a regra**: em linguagem comum. É o **único** campo que o agente lê, e quanto
  mais específica a regra, menos ele erra o momento.
- **Estilo**: **Level Up** (faixa central, três linhas de texto), **Pílula** (no topo, duas linhas,
  a menos intrusiva) ou **Conquista** (cartão lateral com o ícone num quadrado, três linhas).
- **Ícone**: uma grade de doze símbolos, e um campo para digitar o nome de qualquer SF Symbol.
- **Texto de cada parte**: um campo por linha do estilo escolhido. Trocar de estilo não apaga o
  texto que sobra, mas o que sobra não é mostrado.
- **Valores de teste — o que o agente preencheria**: só aparece quando o texto tem marcadores. É
  usado apenas na simulação, e não é gravado.
- **Simular disparo**: chama o anúncio de verdade na sua tela, com os valores de teste. Marcador sem
  valor de teste aparece com o próprio nome, e a simulação ignora a espera descrita abaixo.

## Os marcadores

Um trecho entre chaves no texto (`{versao}`, `{quantos}`) vira um buraco que o agente preenche na
hora de disparar. O nome do marcador aceita letras, números e `_`.

O molde `Release {versao} no ar` vira "Release 1.48.1 no ar" quando o agente dispara passando a
versão. Marcador sem valor vira texto vazio: a chave nunca aparece na tela.

O agente não escreve mais nada. Estilo, ícone e palavras fixas são seus; ele diz qual anúncio
disparar e entrega os valores que faltam.

## Quando o anúncio aparece

O anúncio entra na tela, fica cerca de três segundos e sai. Ele **não** aparece enquanto você está
numa reunião, conversando com a assistente, com o microfone aberto ou com o app falando: nesses
casos ele entra numa fila e aparece assim que você fica livre. Nenhum se perde.

Um por vez, e o mesmo anúncio disparado por vários agentes ao mesmo tempo aparece uma vez só.

## O que os agentes recebem

A lista dos anúncios **ativos**, com nome, regra e os marcadores a preencher, entra no briefing de
cada agente deste projeto no momento em que ele é criado. Um anúncio criado, renomeado ou ativado
depois disso não aparece para os agentes que já estão rodando.

Anúncio sem nome ou sem regra não entra na lista, mesmo ativo.

Não há como pedir um anúncio à assistente por voz: quem dispara é o agente. Veja
[o agente mexe no canvas](o-agente-mexe-no-canvas).

Para os avisos que o próprio app te dá, que são outra coisa, veja [avisos e sons](avisos-e-sons).
