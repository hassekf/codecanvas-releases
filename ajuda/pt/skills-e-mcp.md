---
slug: skills-e-mcp
titulo: Skills e servidores MCP
resumo: O que uma skill e um servidor MCP dão aos agentes deste projeto, e o que dá para pedir a um agente sem abrir tela nenhuma.
area: agentes
nivel: avancado
---

Uma **skill** é um arquivo de instruções que o agente carrega quando o assunto dela aparece. Um
**servidor MCP** é um programa que entrega ferramentas ao agente, como um banco de dados, um issue
tracker ou um serviço da empresa.

As duas coisas se gerem pelas telas ([skills](ajustes-skills), [MCP](ajustes-mcp)) ou pedindo a um
agente. Os dois caminhos mexem no mesmo acervo.

## O que um agente faz com skills

- **Listar**: devolve as skills que este projeto tem à mão, com o nome, a descrição, os programas de
  agente que a enxergam e se ela está ativa neste canvas.
- **Procurar**: busca num registro público por tema, tecnologia ou nome, e devolve os candidatos com
  descrição, estrelas e o repositório de origem. Procurar não instala nada. Se o registro estiver
  fora do ar, o agente avisa.
- **Instalar**: baixa a skill do repositório de origem, no projeto ou na sua conta. O padrão é o
  projeto. Pedida por voz, a instalação vai sempre para o projeto.
- **Escrever**: o agente redige o arquivo da skill inteiro, incluindo o cabeçalho. É por aqui que
  passam "melhora esta skill" e "junta estas três numa só". Uma
  skill com o mesmo nome no mesmo lugar é sobrescrita, e o nome vira o nome da pasta.
- **Ativar e desativar**: vale só neste canvas e só para os agentes iniciados a partir daí. Nada sai
  do disco.
- **Remover**: apaga a skill do disco, sem desfazer. As skills nativas do programa de agente não
  podem ser removidas.

## O que um agente faz com servidores MCP

- **Listar**: devolve os servidores instalados pelo CanvasCode, com o estado de cada um neste canvas,
  e os que você configurou por fora.
- **Buscar**: procura no registro oficial, que é público e não pede conta. O resultado diz o nome
  exato, se o servidor fala por HTTP ou sobe um processo, e se ele pede chave.
- **Instalar**: instala do registro e deixa o servidor ativo só neste canvas. As chaves que ele pedir
  vão para o Keychain do Mac; as que faltarem ficam para você preencher na tela de MCP.
- **Ativar e desativar**: vale para os agentes iniciados a partir de então. Os que já estão de pé
  continuam com os servidores com que nasceram até renascerem.

## Onde uma skill mora

- **Neste projeto**: dentro do repositório, versionada com o código, e portanto disponível a quem
  clonar o projeto.
- **Na sua conta**: vale em todos os seus projetos.
- **Nativa do programa de agente**: vem com ele, e o CanvasCode não a remove.

Ao instalar ou escrever uma skill, você escolhe entre as duas primeiras.

## Desativar não é remover

Desativar pede aos agentes deste projeto para não usarem aquela skill, e desfaz-se num clique.
Remover apaga o arquivo do disco e não tem volta. Para parar de usar uma skill só aqui, desative.

## O que cada servidor custa

- **HTTP**: o servidor é compartilhado e não custa processo nenhum por agente.
- **Processo**: sobe um processo por agente, com cerca de 60 MB cada. Com seis agentes na tela, são
  seis processos daquele servidor.

O servidor MCP do próprio CanvasCode fica fora dessa conta: é um só, dentro do app, compartilhado por
todos os agentes.

## Instalar é deixar código de terceiros rodar

Uma skill traz instruções escritas por outra pessoa, e um servidor MCP traz código que passa a rodar
junto dos seus agentes. O agente confirma a origem com você antes de instalar, e um servidor
instalado por aqui nasce ativo apenas no canvas de onde a instalação partiu.

## Configurado em outra tela

- A lista de skills deste projeto: [ajustes · Skills](ajustes-skills).
- A lista de servidores MCP: [ajustes · MCP](ajustes-mcp).
