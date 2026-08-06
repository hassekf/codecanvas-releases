---
slug: um-agente-chama-outro
titulo: Um agente chama outro
resumo: Delegar por voz, agentes que trazem colegas para o canvas, os painéis de subagente e as conversas entre projetos.
area: agentes
nivel: basico
---

## Você delega

- **Delegar por voz**: entrega a tarefa a um agente deste projeto. Sem um agente livre, o app cria
  um. Dizer o nome manda a tarefa àquele agente, inclusive um que esteja guardado, que volta sozinho
  para receber.
- **Chamar de volta**: traz um agente guardado, com a conversa inteira. Veja
  [criar e fechar](criar-e-fechar).
- **Nome ambíguo não é chutado**: quando dois nomes ficam igualmente prováveis, o app pergunta qual
  deles antes de enviar qualquer coisa.

## Um agente traz colegas

Um agente em trabalho pode abrir outros agentes no canvas, com uma tarefa para cada um. Eles nascem
com painel, terminal e nome próprios, e cada um pode ser de um programa de agente diferente.

- **Abrir sem tarefa** deixa o agente vazio, e nenhum prompt é enviado a ele.
- **Quem abriu recebe o resultado** de cada um ao terminar, inclusive quando a tarefa dá errado.
- **Quem abriu é acordado uma vez**, quando todos os agentes daquele pedido responderem.
- **Quem abriu pode dispensar** os agentes que trouxe. O painel some e a memória fica guardada.
- **Ninguém manda em agente que não trouxe.** Um agente pode ler o que outro recebeu, o que já fez e
  o que disse por último, mas só conversa com quem o trouxe ou com quem ele trouxe.

## Os painéis de subagente

Quando um agente divide o próprio trabalho, cada divisão ganha um painel de atividade com a tarefa
recebida, as ferramentas em uso e a resposta final. O painel permanece depois de concluído, e não é
um terminal.

- **Mostrar subagentes no canvas**, em **Configurações → Agentes**: liga e desliga esses painéis.
  Desligado, os subagentes trabalham igual e o app fecha os painéis que estavam abertos.
- **O botão dos subagentes na barra de comando**: o mesmo interruptor, com o estado à vista.
- **O teto é de três painéis por canvas ao mesmo tempo**, mesmo com o interruptor ligado. Um agente
  pode disparar dezenas de subagentes, e os que passarem do teto trabalham sem painel.
- **Cada painel nasce na área de trabalho do agente que o lançou.**

## Agentes de projetos diferentes

Nenhuma conversa entre projetos começa sozinha.

- **O agente pede licença**: a pergunta aparece na sua tela com quem quer falar com quem, o projeto
  do outro, o motivo e o saldo de mensagens. **Deixar falar** libera; **Não** recusa. A mensagem que
  ele tinha guardada sai no momento em que você autoriza.
- **Você abre uma conversa por voz**, dizendo quem fala com quem e sobre o quê.
- **O que se autoriza é a conversa**, e não cada mensagem: um sim vale para aquele par de agentes,
  aquele assunto e um saldo de mensagens contando os dois lados.
- **O saldo não se renova com o tempo.** Quando ele acaba, a conversa para, e o agente precisa pedir
  mais voltas dizendo o que ainda falta. O pedido chega como uma nova pergunta na sua tela, com
  **Deixar continuar** e **Encerrar**.
- **Conversa entre projetos**, em **Configurações → Agentes**: define o saldo de cada autorização.
  As opções são 2, 4, 6, 10 e 20 mensagens, e o padrão é 4.
- **O cabeçalho do painel** mostra com quem o agente está falando, de que projeto, e quanto do saldo
  já foi gasto. Clicar nesse selo leva até o painel do outro agente.
- **Assunto de produto não atravessa**: escopo, prioridade e decisão do que fazer continuam com você.

## Configurado em outra tela

- Falar com um agente por voz ou por escrito: [falar com eles](falar-com-eles).
- O que um agente pode fazer no canvas: [o agente chama colegas](o-agente-chama-colegas).
- Guardar e trazer de volta um agente: [minimizar e a estante](minimizar-e-a-estante).
