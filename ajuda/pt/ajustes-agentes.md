---
slug: ajustes-agentes
titulo: Configurações dos agentes
resumo: A aba Agentes, controle a controle, e os três ajustes de agente que moram na aba Interface.
area: ajustes
nivel: basico
---

Em **Configurações → Agentes**. O que está aqui vale para todos os projetos. O que é de um projeto só
(a conta em que os agentes dele nascem, o modelo, as permissões, o navegador padrão) fica nas
configurações do canvas. Veja [ajustes do projeto](ajustes-projeto).

- **Histórico de entregas do agente**: ligado, cada assunto concluído vira uma linha no verso do
  painel quando o agente passa ao assunto seguinte. Desligado, o verso mostra só o que ele faz agora.
- **Retomar agentes que a API derrubar**: ligado, o app manda o agente continuar de onde parou depois
  de uma queda da API, esperando mais a cada nova tentativa. O aviso da queda acontece com ele ligado
  ou desligado. Veja [criar e fechar](criar-e-fechar).
- **Hibernar agentes inativos**: desligado por padrão. Ligado, o agente sem atividade pelo tempo
  abaixo é encerrado, o painel fica com um botão de acordar e a conversa é retomada quando ele volta.
  - **Dormir depois de**: aparece dentro do controle acima, e só com ele ligado. Vai de 5 minutos a 8
    horas, e vem em 1 hora. O relógio zera a cada ferramenta usada, a cada prompt enviado e sempre
    que você abre o painel do agente. Nunca dormem quem está trabalhando, quem espera resposta sua e
    o painel selecionado no canvas em foco.
- **Instalações do Claude**: cadastra pastas `.claude`, cada uma com o próprio login, servidores e
  conversas. **Adicionar instalação…** pede a pasta. Tirar da lista não apaga nada do disco, e o app
  pergunta o que fazer com os agentes que dependiam dela. Veja [contas e perfis](contas-e-perfis).
- **Versão do Claude Code**: **A mais recente** mantém o Claude Code atualizado sozinho na abertura
  do app, antes de qualquer agente nascer. O menu também lista as versões presentes na máquina, e
  fixar uma desliga a atualização automática. A troca vale para os agentes criados dali em diante.
- **Selo de pull request**: mostra o PR de cada agente no painel, no rodapé e no Git, com o estado da
  integração contínua. Desligado, o app deixa de consultar o GitHub sobre os seus PRs. Ver
  [o painel do Git](painel-git).
- **Dev servers em painel próprio**: desligado por padrão. Ligado, comandos longos como um servidor
  de desenvolvimento ou um observador de arquivos são abertos num painel de terminal visível, em vez
  de rodarem dentro do agente. Veja [falar com eles](falar-com-eles).
- **Isolamento por worktree**: ligado, cada agente cria a própria cópia do projeto antes de escrever
  e comita na branch dele. O texto do protocolo que os agentes recebem é editável logo abaixo, e o
  editor só aparece com o interruptor ligado. Ver
  [worktrees e isolamento](worktrees-e-isolamento).
- **Painéis de subagente**: **Mostrar subagentes no canvas** dá um painel a cada tarefa que um agente
  delega, até três ao mesmo tempo. Desligado, os subagentes continuam trabalhando sem aparecer. Ver
  [um agente chama outro](um-agente-chama-outro).
- **Conversa entre projetos**: quantas mensagens uma autorização sua libera entre um agente daqui e
  um agente de outro projeto. As opções são 2, 4, 6, 10 e 20 mensagens, e o padrão é 4. Esgotadas,
  eles precisam de uma autorização nova.

## Na aba Interface

- **Brilho no painel ao terminar**: a moldura do painel brilha quando o agente entrega, mesmo sem
  ele estar selecionado.
- **Destacar a aba da área ao terminar**: a aba da área pisca quando um agente termina, ou passa a
  esperar você, numa área que você não está vendo.
- **Cor do brilho de conclusão**: a cor dos dois anteriores. O botão **Padrão** só aparece depois de
  você trocá-la, e a devolve.
- **Agrupar os agentes em abas**, na seção **Barra de frentes**: numa área com mais de um agente,
  eles dividem um painel, com o escolhido à mostra e os outros em abas. Vale para as áreas que nunca
  foram configuradas à mão; o menu de contexto de cada área manda por cima. Ver
  [áreas de trabalho](areas-de-trabalho).
- **Esconder as abas de área quando ela estiver encaixada**, na mesma seção: as abas do topo somem e
  a barra de frentes passa a listar as áreas, trocar no clique, criar, renomear e piscar. O controle
  só funciona com a barra encaixada.
