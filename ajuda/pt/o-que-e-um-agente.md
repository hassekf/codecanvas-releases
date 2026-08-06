---
slug: o-que-e-um-agente
titulo: O que é um agente
resumo: Um CLI de agente rodando num terminal de verdade dentro do painel, na pasta do canvas, com nome próprio.
area: agentes
nivel: basico
---

Um agente é um CLI de agente (Claude Code, Codex, Grok ou opencode) rodando num terminal de verdade
dentro de um painel do canvas.

## O que roda ali dentro

- **O programa inteiro**: os comandos de barra, o seletor de modelo, os diffs e os pedidos de
  permissão são os do próprio CLI, e você digita neles como digitaria no Terminal.
- **A configuração que já está no projeto**: as instruções escritas na pasta, os servidores MCP e os
  subagentes são lidos pelo CLI, que roda na pasta do canvas.
- **O binário instalado nesta máquina**: o app procura cada CLI no `PATH` e mostra em
  **Configurações → Provedores** qual encontrou. Veja [vários provedores](varios-provedores).

## A pasta

O diretório de trabalho não é escolhido na criação: ele vem do canvas, e todo agente criado ali
nasce nele. Veja [escolher o projeto](escolher-o-projeto).

## O nome

O nome é escolhido na criação, com uma sugestão já preenchida, e é por ele que você endereça o
agente na voz, no `⌘K` e no painel de elenco.

- **Enquanto o agente existir no projeto**, na tela ou guardado, o nome dele fica reservado e nenhum
  agente novo pode recebê-lo.
- **Esquecer um agente devolve o nome** ao conjunto de nomes disponíveis. Ver
  [criar e fechar](criar-e-fechar).

## Permissões

Nas configurações do canvas, em **Como os agentes nascem**, está o interruptor **Não pedir
permissão**, ligado por padrão. Desligado, o CLI volta a pedir licença antes de cada ferramenta, o
agente fica no estado de espera enquanto o pedido não for respondido, e você é avisado. O menu **Modo
de permissão** só aparece com ele desligado. Veja [ajustes do projeto](ajustes-projeto).

## O navegador dele

Um agente pode abrir um navegador no canvas, e aquele painel pertence a ele: nenhum outro agente
navega, clica ou fotografa ali. Veja [o agente vê o navegador](o-agente-ve-o-navegador).

## O painel e o agente são coisas diferentes

Fechar o painel dispensa o agente e guarda a conversa, o nome, a última tarefa e o que ele registrou
ter entregado. Veja [criar e fechar](criar-e-fechar).
