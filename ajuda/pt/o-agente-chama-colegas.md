---
slug: o-agente-chama-colegas
titulo: O agente chama colegas
resumo: Trazer outros agentes, ler o que os vizinhos fizeram, devolver resultado e falar com um agente de outro projeto.
area: agentes-fazem
nivel: basico
---

## O que pedir

- *"Sobe três agentes e divide as telas entre eles."*
- *"Chama um Codex para revisar isso, quero a opinião de outro modelo."*
- *"Antes de começar, vê o que o Circe descobriu sobre esse bug."*
- *"Quem já trabalhou nessa parte do projeto?"*
- *"Isso depende do formato que o backend devolve. Pergunta pro pessoal de lá."*

Para o lado que parte de você, veja [um agente chama outro](um-agente-chama-outro).

## Trazer agentes

Um agente cria outros agentes no canvas, um painel por agente, com terminal próprio.

- **A tarefa é opcional.** Com tarefa, o agente novo nasce com o pedido já enviado. Sem tarefa, ele
  nasce vazio e nenhum prompt é mandado.
- Cada agente novo pode ser de outro programa: Claude Code, Codex, Grok ou opencode. Veja
  [vários provedores](varios-provedores).
- Todas as tarefas saem numa chamada só. Quem delegou encerra o turno e é acordado uma vez, quando
  todos responderem, com as respostas juntas.
- **Isto é diferente dos subagentes internos**, que não aparecem no canvas, usam o mesmo modelo e
  respondem dentro do mesmo turno. Um agente do canvas tem memória própria, que sobrevive à conversa
  que o criou.

## Ler os colegas

- **Ler um agente**: a tarefa que ele recebeu, o que já fez e o que disse por último. Qualquer agente
  do projeto pode ler qualquer outro.
- **Listar os agentes do projeto**: os que estão na tela e os que foram dispensados, com a última
  missão de cada um.

## Falar com os colegas

A mensagem só alcança quem tem vínculo: quem o agente trouxe, e quem o trouxe.

- **É por aí que o resultado volta.** Um agente que recebeu tarefa de outro responde por essa via ao
  terminar, inclusive quando deu errado.
- A mensagem carrega um resumo curto e o caminho dos arquivos produzidos, não o conteúdo deles.
- Nenhum agente manda tarefa para quem ele não trouxe.

## Dispensar

Um agente fecha os agentes que ele mesmo trouxe. O painel sai da tela e a memória fica guardada: você
pode chamar o agente de volta pelo [elenco](painel-elenco) ou pelo `⌘K`. Um agente não dispensa quem
não foi ele que abriu.

## Falar com um agente de outro projeto

**Nenhuma conversa entre projetos começa sozinha.** O agente pede, a pergunta aparece na sua tela com
o assunto e a mensagem já escritos, e você autoriza ou recusa. Recusado, ele é avisado e segue.

- O que você autoriza é a **conversa**: um par de agentes, um assunto e um saldo de mensagens.
- **O saldo padrão é de 4 mensagens**, e o menu em Configurações → Agentes → "Conversa entre
  projetos" oferece 2, 4, 6, 10 ou 20. O ajuste é global, não por projeto.
- O saldo não se renova com o tempo. Quando acaba, a conversa para. O agente pode pedir mais
  mensagens, explicando o que exatamente falta para fechar, e a decisão volta a ser sua.
- Depois de pedir, o agente encerra o turno. Ele é acordado quando houver resposta.
- Você também pode abrir a linha sem esperar o pedido: *"deixa o Tristão falar com o Ares do
  backend"*.

O que atravessa é fato do sistema e acordo entre as duas pontas: o formato do payload, o nome do
campo, a unidade, quem valida o quê. Escopo, prioridade e o que a funcionalidade faz não atravessam:
essas perguntas voltam para você.
