---
slug: o-agente-usa-suas-listas
titulo: O agente usa as suas listas
resumo: O que um agente lê e escreve nas suas tarefas, nas suas notas e nos seus recados, e o que ele não consegue fazer nelas.
area: agentes-fazem
nivel: basico
---

## O que pedir

- *"Vê na lista se isso já está anotado antes de começar."*
- *"Pega a próxima tarefa e trabalha nela."*
- *"Marca como feita e comenta o que você fez."*
- *"Anota na nota das chaves o token novo do servidor de testes."*
- *"Responde o recado do Bruno contando que já está no ar."*

## As tarefas

Veja [o painel de tarefas](painel-tarefas).

- **Ler a lista**: o que falta, com prazo, estado e quem mexeu em cada tarefa. As concluídas só
  aparecem se ele pedir por elas.
- **Criar**: texto e, quando você disser um, prazo em `AAAA-MM-DD`, com hora opcional.
- **Atualizar**: estado (aberta, fazendo, feita), comentário, texto e prazo. Só o que mudou é
  enviado.
- **Apagar**: a tarefa vai para a lixeira, de onde você a restaura pelo painel. O histórico registra
  que foi o agente quem apagou.

O que a lista não mostra:

- **Cada comentário é assinado com o nome do agente que o escreveu.** Ele não escolhe a assinatura,
  não assina como outro agente e não assina como você.
- **Concluir e apagar são coisas diferentes.** "Já está feito" é o estado `feita`, com um comentário
  do que foi feito. Apagar é só quando você pede.
- Os agentes são instruídos a não reorganizar a lista, não decidir prioridade e não usá-la como
  caderno próprio.

## As notas

Veja [o painel de notas](painel-notas).

- **Ler**: sem apontar qual, ele recebe os títulos. Apontando o título ou um trecho, ele recebe o
  texto inteiro daquela nota.
- **Criar**: com título, ou sem, e aí a primeira linha do texto vira o nome.
- **Atualizar**: ele acrescenta texto ao fim, numa linha nova, ou renomeia a nota.

**Não existe caminho para um agente reescrever nem apagar o que está numa nota.** Apagar uma nota é
gesto seu, no painel.

## Os recados

Os recados vão para outra pessoa, em outro computador. Veja [o painel de recados](painel-recados).

- **Listar contatos**: quem você já adicionou, e quem mandou recado ainda não lido. A lista vem
  numerada.
- **Ler os recados**: sem apontar de quem, os não lidos. **Ler por essa via marca como lido**, e o
  painel deixa de mostrar o recado como novo. Anexos não vêm no texto: eles são citados pelo nome, e
  quem os abre é você.
- **Responder** um recado que chegou, e **mandar** um recado novo, com assunto e corpo.
- Um arquivo pode ir junto do recado: o que viaja é o conteúdo, com teto de 5 MB, e não o caminho.

Restrições:

- Um agente só manda recado para quem está nos seus contatos. Ninguém é encontrável por busca.
- **Quem nunca definiu o próprio nome aparece como "sem nome"**, e o número da lista é a única forma
  de endereçar essa pessoa.
