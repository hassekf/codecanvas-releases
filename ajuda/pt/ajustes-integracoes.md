---
slug: ajustes-integracoes
titulo: Integrações
resumo: A agenda do Mac nas Configurações, o que a Nina vê dela, e por que o Jira se conecta na edição do projeto.
area: ajustes
nivel: basico
---

Em **Configurações → Integrações**.

## A agenda do Mac

- **Conectar a agenda**: traz os compromissos de todas as contas que o seu Mac já tem, incluindo
  iCloud, Google e Exchange. O app só lê a agenda; nunca escreve nada nela. Ao ligar, o macOS pede a
  permissão. Se você negar, o interruptor volta para desligado.
- **O macOS negou o acesso**: aparece embaixo do interruptor quando a permissão foi negada. O macOS
  não pergunta de novo sozinho, e **Abrir Ajustes do Sistema** leva à tela de Calendários. As outras
  permissões estão em [as permissões que o macOS pede](permissoes-do-mac).

Desligada, a agenda não existe para o app: nada na tela inicial, nenhum aviso, e a Nina não recebe a
ferramenta de agenda.

Ligada, aparecem os controles abaixo.

- **O que a Nina pode ver**: cinco interruptores, um por dado do compromisso (o título, o local, a
  descrição e a pauta, os participantes e o link da chamada). Só o que estiver ligado sobe para a
  OpenAI, e só quando você pergunta à Nina sobre a agenda. Os compromissos mostrados na tela do app
  não saem do seu Mac. O link da chamada é o que ela precisa para abrir a reunião por voz.
- **Quais agendas entram**: um interruptor por calendário que o Mac tem, com a conta de cada um.
  Nenhum marcado quer dizer todos; a primeira desmarcação materializa a lista.
- **Avisar antes da reunião**: o aviso aparece antes do começo e fica até você entrar ou dispensar.
- **Avisar antes**: 5, 10, 15 ou 30 minutos antes. Só aparece com o aviso ligado.
- **Ao abrir uma reunião**: **Num painel daqui**, que abre a chamada num navegador do canvas já
  logado na sua conta do Google, ou **No meu navegador**. Você pode trocar na hora, no próprio aviso.

O que acontece no dia da reunião está em [agenda e reuniões](agenda-e-reunioes).

## Atlassian

O Jira e o Confluence não se conectam aqui: a conexão é de cada canvas.

- **Jira de "<nome do projeto>"**: com um projeto aberto, o botão **Conectar** ou **Editar** abre a
  edição daquele workspace já na parte da Atlassian. O texto ao lado diz se ele já está conectado.
- **Nenhum workspace aberto**: sem projeto aberto não há o que conectar, e a tela diz isso.

O passo a passo está em [Jira e Confluence](jira-e-confluence).

## Onde ficam os segredos

Toda credencial de integração fica no Keychain do seu Mac, nunca num arquivo do app, e desconectar
apaga a credencial junto.
