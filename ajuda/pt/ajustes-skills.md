---
slug: ajustes-skills
titulo: Ajustes · Skills
resumo: A tela que lista as skills à mão deste projeto, liga e desliga cada uma aqui, e instala do registro público.
area: projeto
nivel: avancado
---

Em **Editar o projeto → Skills**. A aba só existe num projeto já criado.

## A lista

As skills vêm agrupadas por origem, e cada linha traz o nome, a descrição e uma etiqueta por programa
de agente que a enxerga.

- **Neste projeto**: estão no repositório e são versionadas com o código.
- **Global do provedor**: estão na sua conta e valem em todos os seus projetos.
- **Do sistema**: nativas do programa de agente. Vêm marcadas com um cadeado, abrem em leitura e não
  podem ser removidas.
- **Sem nenhum programa de agente instalado na máquina**, a aba diz isso e não lista nada: não há de
  onde descobrir skills.

## O interruptor de cada linha

- **Desligar** pede aos agentes deste projeto para não usarem aquela skill, e vale para os agentes
  iniciados a partir daí. Quem já está de pé continua como nasceu.
- **A skill desligada continua na lista**, esmaecida, e nada sai do disco.
- **O efeito é só deste canvas.** A mesma skill continua valendo nos seus outros projetos.

## O menu de cada linha

- **Ver / editar SKILL.md**: abre o arquivo da skill para leitura e edição. Nas do sistema, só
  leitura.
- **Remover…**: apaga a skill do disco, incluindo os atalhos que a compartilhavam entre programas de
  agente. Pede confirmação e não tem desfazer. Para parar de usá-la apenas aqui, use o interruptor.

## Instalar

**Instalar skills…**, no topo da aba, abre a busca no registro público.

- **O campo de busca** filtra por tema, tecnologia ou nome, e cada resultado traz descrição,
  estrelas e o repositório de origem.
- **Escolher um resultado** abre a confirmação, com o link para o repositório. É código de terceiros,
  e a origem se confere ali.
- **Onde instalar**: **Neste projeto**, versionada no repositório, ou **Na minha conta**, valendo em
  todos os seus projetos.
- **Com o registro fora do ar**, a janela diz isso em vez de continuar procurando.
- **A instalação falha** quando o repositório é privado, está fora do ar, ou não tem o arquivo da
  skill no caminho indicado. O motivo aparece na própria janela.

## Configurado em outra tela

- O que uma skill é, e o que dá para pedir a um agente: [skills e MCP](skills-e-mcp).
- Os servidores de ferramentas deste projeto: [ajustes · MCP](ajustes-mcp).
