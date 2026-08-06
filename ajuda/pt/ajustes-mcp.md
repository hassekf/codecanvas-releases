---
slug: ajustes-mcp
titulo: Ajustes · MCP
resumo: A tela que escolhe os servidores MCP que os agentes deste projeto sobem, instala novos do registro oficial e diz o que cada um custa.
area: projeto
nivel: avancado
---

Em **Editar o projeto → MCP**.

## Instalados por aqui

Os servidores que vieram do registro, pelo CanvasCode.

- **O interruptor** liga o servidor neste canvas. Cada servidor instalado nasce ativo apenas no
  canvas de onde a instalação partiu, e dormente nos demais.
- **Desinstalar…**, no menu da linha: tira o servidor do acervo do app.

## Já configurados

Os servidores que você instalou por fora, na sua conta do programa de agente ou no próprio projeto.
O CanvasCode não os altera: aqui só se escolhe usá-los ou não neste canvas.

- **Todos vêm ligados.** Desligar um deixa de subi-lo para os próximos agentes deste projeto.
- **Religar todos** volta ao estado de herdar a lista inteira, e um servidor novo que você configurar
  por fora entra sozinho.
- **Sem nenhum servidor configurado por fora**, a seção diz isso.

## O que cada um custa

Cada linha traz uma etiqueta.

- **HTTP**: o servidor é compartilhado e não custa nada por agente.
- **Processo**: sobe um processo por agente, cerca de 60 MB cada. Com seis agentes na tela, são seis.

O servidor MCP do próprio CanvasCode, que dá ao agente os painéis, o navegador e as suas listas, não
entra nessa conta: é um só, dentro do app, compartilhado por todos os agentes.

## Instalar

**Instalar…**, no topo, busca no registro oficial, que é público e não pede conta.

- **Cada resultado** diz se o servidor fala por HTTP ou sobe um processo, e se ele pede chave.
- **A confirmação** mostra o custo, o link para o código-fonte e os campos que ele precisa, com os
  obrigatórios marcados. O botão de instalar fica indisponível enquanto faltar um obrigatório.
- **As chaves vão para o Keychain do seu Mac**, nunca para um arquivo, e são entregues ao servidor
  apenas na hora de subir o agente.
- **Instalado a partir de um projeto**, o servidor fica ativo nele e dormente nos outros.

## Salvar reinicia os agentes parados

Ao salvar uma mudança de servidores, os agentes parados deste canvas renascem com a lista nova, e o
app diz quais foram.

- **Renascer não é recomeçar**: eles voltam com a conversa inteira e o mesmo lugar no canvas. O que
  se perde é o histórico já pintado na tela do terminal.
- **Quem está trabalhando não é tocado.** Esses agentes pegam os servidores novos na próxima vez que
  renascerem.

## Configurado em outra tela

- O que um servidor MCP é, e o que dá para pedir a um agente: [skills e MCP](skills-e-mcp).
- As instruções que os agentes carregam: [ajustes · Skills](ajustes-skills).
