---
slug: permissoes-do-mac
titulo: As permissões que o macOS pede
resumo: Cada permissão que o sistema pergunta, o que ela libera, o que quebra ao negar, e como fazer o Mac perguntar de novo.
area: comecando
nivel: basico
---

O macOS pergunta na primeira vez que você usa cada recurso. Nenhuma delas é pedida no arranque.

## As permissões

- **Microfone**: sem ele, a conversa por voz e o ditado não funcionam. Veja
  [configurar a voz](configurar-a-voz).
- **Reconhecimento de fala**: usado pelo ditado que roda no próprio Mac. Veja [ditado](ditado).
- **Gravação de tela**: sem ela, gravar a janela do app não funciona. Veja
  [o painel de gravação](painel-gravacao).
- **Câmera**: a imagem aparece no [painel de webcam](painel-webcam-e-avatar) e não sai do seu Mac.
- **Calendário**: o app lê a sua agenda para avisar das reuniões e abrir o link da chamada. Nada é
  escrito no seu calendário. Veja [agenda e reuniões](agenda-e-reunioes).
- **Notificações**: os avisos do macOS quando o app está em segundo plano. O pedido só é feito depois
  que você liga "Avisar no Mac fora do app" em [avisos e sons](avisos-e-sons).
- **Mesa, Documentos e Downloads**: as pastas em que os agentes leem e escrevem.

## O acesso às pastas

**O macOS cobra a permissão do CanvasCode, e não do programa do agente.** Um agente aberto aqui
dentro é um processo filho, e o sistema atribui o acesso ao responsável.

Negar não produz um pedido de permissão no terminal do agente. Ele recebe um erro de acesso negado, e
com frequência conclui que o arquivo não existe.

Para liberar depois: Ajustes do Sistema → Privacidade e Segurança → Arquivos e Pastas, e habilite o
CanvasCode para a pasta em questão.

## Quando o macOS parou de perguntar

Uma permissão negada não é perguntada de novo: o pedido responde "não" na hora, sem diálogo. Isso
acontece também quando existe um registro antigo deste app feito por um binário com outra assinatura,
como uma build de desenvolvimento ou uma versão anterior.

Em **Configurações → Diagnóstico** ficam:

- o estado de **Microfone**, **Reconhecimento de fala** e **Gravação de Tela**;
- **Pedir permissão**, que só faz efeito enquanto o sistema ainda não decidiu;
- **Abrir Ajustes do Sistema** e **Gravação de Tela nos Ajustes**, que levam a cada painel do
  sistema;
- **Reconferir**, que relê o estado;
- **Apagar as permissões e perguntar de novo**, que aparece quando alguma está negada. Ele apaga o
  registro de permissão deste app, e de nada mais. **O app precisa ser reaberto depois**, e as
  perguntas voltam do zero.
