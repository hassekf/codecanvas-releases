---
slug: painel-git
titulo: O painel do Git
resumo: As três abas do repositório: o que está na sua pasta, as issues e as pull requests, com o que cada botão faz.
area: paineis
nivel: basico
---

O repositório do projeto em três abas: **Git**, **Issues** e **PRs**. Cada aba mostra a contagem do
que ela tem; quando a contagem é zero, o número não aparece.

Abra pelo `⌘K` digitando "git", ou clicando no indicador de branch no rodapé. O painel é um por
canvas: pedir de novo traz para a frente o que já existe.

## O indicador do rodapé

- **A branch atual**, truncada no meio quando é longa.
- **Setas**: quantos commits você está à frente e atrás do remoto. Aparecem só quando há
  divergência.
- **A contagem de arquivos mudados**, com o total de linhas somadas e removidas, ou a palavra
  "limpo" quando não há nada por commitar.
- **"N disputados"**, quando algum arquivo mudado tem mais de um autor.
- **Clicar** abre este painel.

## A aba Git

O cabeçalho traz a branch, as setas de divergência com o remoto, o selo da pull request desta branch
e o botão de recarregar. Sem um remoto configurado, as setas não aparecem. Fora de um repositório, a
aba diz que o workspace não é um repositório git.

- **Mudanças**: os arquivos alterados e ainda não commitados. Cada linha traz a letra do estado, o
  caminho, quantas linhas entraram e saíram, e o nome de quem mexeu no arquivo, inclusive antes de
  qualquer commit. A sua própria edição num [painel de arquivo](painel-arquivo) conta como autoria.
- **Arquivo disputado**: o que tem dois ou mais autores ganha um alerta na linha. A ordem da lista é
  conflitos primeiro, disputados depois, e o resto por caminho.
- **Commits**: os 25 últimos, com resumo, autor e quando. O commit criado por um agente nesta sessão
  aparece com o nome do agente; os demais mostram o autor registrado no git, que é você mesmo em
  todos eles.
- **Diff**: clicar num arquivo mudado abre o diff no lugar da lista. A seta no canto superior volta.

## A aba Issues

As issues abertas do repositório.

- **O filtro no topo** recorta por etiqueta. **Todas** desliga o recorte.
- **Clicar numa issue** expande as ações, as etiquetas e a descrição.
- **Trabalhar nisto**: abre um agente novo com a issue montada como tarefa inicial. Com mais de um
  provedor ligado, o botão vira um menu de qual abrir.
- **Mandar para…**: entrega a mesma tarefa a um agente já aberto neste canvas. Sem agente aberto, o
  botão não aparece.
- **Fechar**: marca a issue como resolvida no GitHub.
- **Abrir no app** abre a issue num [painel de navegador](painel-navegador); **Abrir no GitHub** abre
  no navegador do sistema.

O texto entregue por **Trabalhar nisto** e por **Mandar para…** é o mesmo, e ele instrui o agente a
comentar e fechar a própria issue ao terminar.

## A aba PRs

As pull requests abertas.

- **Todas** e **Esperando você**: o segundo recorta as que estão travadas na sua revisão.
- **Fechada**, cada linha traz número, título, o selo da revisão (**Aprovada**, **Mudanças**,
  **Aguardando**) e o da CI, quando a PR tem CI.
- **Clicar** expande, e só então o app busca a descrição e os arquivos, que a listagem não traz.
- **Aprovar**: pede confirmação e publica a aprovação no GitHub. Fica indisponível numa PR que você
  já aprovou.
- **Comentar**: abre um campo de texto. **Enviar** publica um comentário solto, que não vira
  revisão.
- **Os arquivos alterados** aparecem com o saldo de linhas de cada um. Clicar em qualquer um deles
  abre os arquivos da PR no navegador.

Mergear e pedir mudanças não existem neste painel.

## O selo de pull request

Quando a branch de um agente já virou PR, o número dela e o estado da CI aparecem no painel do
agente, no rodapé e no cabeçalho da aba Git. Sem PR aberto, o selo não ocupa espaço.

O interruptor é **Selo de pull request**, em [configurações dos agentes](ajustes-agentes).
Desligado, nenhum selo aparece e o app deixa de consultar o GitHub sobre as suas PRs.

## O que as abas Issues e PRs exigem

Elas falam com o GitHub pelo `gh`, a ferramenta de linha de comando dele, usando o login que já
existe nela. Quando algo falta, a aba diz qual das três coisas é: o `gh` não instalado, o `gh` sem
login, ou o projeto sem um remoto do GitHub.
