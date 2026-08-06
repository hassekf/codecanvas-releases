---
slug: iniciativas-escrever
titulo: Escrever uma Iniciativa
resumo: Os dois caminhos para criar o arquivo do processo conversando com um agente, e como mudá-lo depois.
area: iniciativas
nivel: avancado
---

Você não preenche formulário nenhum: **quem escreve o arquivo é um agente, conversando com você**. O
painel de Iniciativas abre a conversa e diz ao agente onde gravar.

## Os dois caminhos

Os dois estão na tela do painel quando o projeto ainda não tem nenhuma Iniciativa, e em **Nova
iniciativa** depois disso. Nos dois você escolhe qual agente recebe, e a conversa acontece no painel
dele.

### Escrever do zero, conversando

O agente **não lê o projeto e não propõe nada** ao ser aberto. Ele responde uma linha dizendo que
está pronto e espera você contar qual processo quer descrever.

A partir daí ele pergunta o que faltar, em vez de preencher por conta própria: as etapas na ordem, o
que cada uma produz, o que barra, e onde alguém aprova. Ele só grava o arquivo quando o processo
estiver fechado com você.

É o caminho para um processo que existe na sua cabeça, ou que ainda vai existir.

### Ler o projeto e propor

O agente recebe junto o que o painel já encontrou no repositório sem ler nada: os comandos, os
scripts de validação e as execuções antigas. Ele lê esses arquivos, monta a esteira a partir do que
**está escrito**, pergunta o que faltar em vez de inventar, grava e então te conta em cinco linhas o
que entendeu, para você conferir se bate com o que o time faz de verdade.

É o caminho para um processo que já está no projeto, espalhado em scripts.

## O que o arquivo descreve

O agente escreve isto; vale saber o que ele vai te perguntar:

- **Como uma run começa**: o que a Iniciativa exige para começar — uma fonte, um texto, uma lista de
  perguntas, a saída de outra run, ou nada.
- **Os passos, em ordem**: o nome de cada um, o que entra, o que sai, e quem executa (um comando ou
  um agente com a instrução dele).
- **O portão de um passo**: o comando que prova que o resultado serve. Sem portão, o passo passa com
  a palavra do agente.
- **A assinatura**: o momento em que a run para e espera você, com o que ela mostra e o rótulo do
  botão de aprovar.
- **A revisão**: um passo cuja saída é um veredito, que aprova, reprova ou barra o trabalho.
- **O teto de voltas** de cada rota de conserto.

## Mudar depois

Na tela da Iniciativa:

- **Editar com um agente**: manda o arquivo e o que você quer mudar ao agente que escolher.
- **Ver as origens**: os arquivos do projeto de onde a Iniciativa saiu, cada um marcado como
  **aponta** (a run lê a versão de agora) ou **cópia** (a run usa a versão gravada na Iniciativa).
- **Ver o que mudou**: aparece quando um arquivo de origem mudou depois que a Iniciativa foi escrita.
  **Reler com o agente** manda a ele o arquivo, o que mudou e a Iniciativa que veio dali; ele lê e
  responde o que ficou desatualizado, sem mexer em nada.

**Editar a Iniciativa com uma run andando muda a execução em curso**, e a tela da run avisa quando
isso aconteceu.

## Quando o arquivo tem erro

Um arquivo que o app não conseguiu ler aparece na lista mesmo assim, marcado, e a tela dele lista
cada recusa com o campo e o motivo. O menu oferece **Ver os problemas**, **Pedir a um agente que
conserte** e **Abrir o arquivo**.

## Por onde seguir

- O conceito e o vocabulário: [o que é uma Iniciativa](iniciativas-o-que-e).
- Rodar e acompanhar: [o painel de Iniciativas](painel-iniciativas).
