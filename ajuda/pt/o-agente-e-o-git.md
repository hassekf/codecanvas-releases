---
slug: o-agente-e-o-git
titulo: O agente e o repositório
resumo: Ler o estado do repositório com a autoria do que ainda não foi commitado, resolver issues e revisar pull requests do GitHub.
area: agentes-fazem
nivel: avancado
---

## O que pedir

- *"Antes de mexer nesse arquivo, vê se tem alguém nele."*
- *"Me diz o que ainda não foi commitado e o que cada um andou mexendo."*
- *"Pega a primeira issue e resolve. Comenta a causa e fecha quando o conserto estiver commitado."*
- *"O que está esperando a minha aprovação?"*
- *"Lê a PR 214 e me diz se dá para aprovar."*

## Ler o repositório

Um agente lê a branch atual, o que ainda não foi commitado e os últimos commits.

**Junto vem o que o git não tem: qual agente escreveu em cada arquivo ainda não commitado.** O
CanvasCode registra a autoria das edições feitas pelos agentes deste canvas, e a leitura aponta
quando dois agentes estão no mesmo arquivo.

- Nesse caso não há conflito para o git detectar, porque nada foi commitado. Quem salvar por último
  sobrescreve o outro.
- O mesmo relatório aparece para você em [o painel do Git](painel-git).
- A saída para trabalho pesado em paralelo é cada agente na própria cópia do projeto, em
  [worktrees e isolamento](worktrees-e-isolamento).

## As issues do GitHub

- **Listar** as issues abertas: título, labels e prévia. Um filtro por label reduz a lista.
- **Ler uma issue inteira**, com o corpo completo, pelo número.
- **Comentar**, **renomear** e **fechar**, com um comentário de fechamento opcional.
- **Reabrir** uma issue fechada, com o motivo.

Os agentes são instruídos a comentar a causa real e não só "resolvido", a renomear o título quando
ele descreve apenas o sintoma reportado, e a fechar quando o conserto estiver commitado ou quando
concluírem que não era um bug.

As issues do Jira são outra coisa, e ficam em [o painel do Jira](painel-jira).

## As pull requests

- **Listar** as PRs abertas: título, autor, branch, estado da revisão e estado da CI.
- **Ler uma PR inteira**, com a descrição e os arquivos alterados, pelo número.
- **Filtrar** pelas que pedem a sua revisão.
- **Aprovar**, publicando um review de aprovação no GitHub, com comentário opcional.
- **Comentar**, sem aprovar.

**Pedir mudanças e fazer merge não existem por aqui.** O merge continua sendo seu, ou do agente no
terminal dele.

## O que isso exige

As issues e as pull requests vêm do GitHub pelo `gh`, com o login que já está na máquina. Faltando
alguma peça, o agente recebe qual das três é:

- o `gh` não está instalado;
- o `gh` está instalado e ninguém fez login;
- o projeto não tem um remote do GitHub.

## O que não existe por aqui

- Commitar, criar branch e fazer merge não são ações do canvas. O agente faz isso no terminal dele,
  como faria fora do app.
- Um agente enxerga o repositório do projeto em que ele vive, e só ele.
