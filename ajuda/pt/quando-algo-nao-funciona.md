---
slug: quando-algo-nao-funciona
titulo: Quando algo não funciona
resumo: Sintoma e ação: o que fazer diante de cada falha comum do CanvasCode, e onde o app já mostra a causa.
area: conta
nivel: basico
---

## O painel do agente não abre nenhum terminal

O painel diz qual é o caso.

- **"O Claude Code não está instalado."**: clique em **Instalar agora**. A instalação é local e não
  pede senha de administrador. Veja [o primeiro agente](primeiro-agente).
- **Outro CLI declarado como não instalado**: o painel mostra o comando de instalação dele. Rode o
  comando num terminal e reabra o app. Veja [vários provedores](varios-provedores).
- **"Preparando o agente…"**: o app está perguntando ao shell onde mora o CLI. Espere alguns
  segundos.

## Um agente parou no meio e parece que terminou

É o provedor derrubando o agente. O app avisa com uma notificação que não some sozinha e, com a
retomada automática ligada, manda o agente continuar, espaçando cada nova tentativa. Ele não insiste
diante de credencial recusada, serviço fora do ar ou conversa cheia demais.

- **Para ligar ou desligar a retomada**: **Retomar agentes que a API derrubar**, em
  [configurações dos agentes](ajustes-agentes). Desligada, a queda continua sendo mostrada e
  anunciada, e você retoma pelo botão do aviso, por voz, ou digitando no terminal do agente.
- **Para saber se isso está acontecendo demais**: **Configurações → Diagnóstico**, em **Quedas por
  erro de API**. São os últimos sete dias, por provedor, com quantas foram retomadas sozinhas e um
  gráfico por dia. **Limpar registro** zera a contagem.

## Não sei se o problema é meu ou do provedor

No rodapé, o selo de cada provedor mostra o estado do serviço dele. Passe o mouse para ler o recado,
e clique para abrir a página de estado num painel de navegador.

## Um agente voltou sem lembrar de nada

A conversa de um agente mora dentro da conta em que ele nasceu. O app avisa em qual conta procurou
e, quando a conversa está em outra conta cadastrada, diz qual é.

**Troque a conta daquele agente** para trazer a conversa: clique direito no painel dele e escolha em
**Conta do agente**. O app não move a conversa sozinho. Veja [contas e perfis](contas-e-perfis).

## Um agente diz que não tem permissão para ler um arquivo

O macOS cobra do CanvasCode a permissão de acesso a Documentos, Área de Trabalho e Downloads, e o
agente recebe apenas um erro de acesso negado.

Libere em **Ajustes do Sistema → Privacidade e Segurança → Arquivos e Pastas**. Veja
[as permissões que o macOS pede](permissoes-do-mac).

## A Nina não te ouve

1. Abra **Configurações → Diagnóstico** e leia o estado do **Microfone**: *liberado*, *negado*,
   *bloqueado* ou *nunca perguntado*.
2. Em *nunca perguntado*, clique em **Pedir permissão**.
3. Em *negado* ou *bloqueado*, clique em **Apagar as permissões e perguntar de novo**. O macOS não
   pergunta duas vezes, e este botão apaga o registro de permissão deste app para que ele volte a
   perguntar. O app se reabre em seguida, e nada mais é apagado.
4. Estando *liberado*, confira o **Microfone** em **Configurações → Voz** e use **Testar o
   microfone**, logo abaixo. Medidor parado em zero costuma ser o macOS captando de outro
   dispositivo.

Se ela parar de ouvir no meio de uma conversa que estava funcionando, o indicador de voz mostra
"reconectando…" e a conexão volta sozinha. Mais em [configurar a voz](configurar-a-voz).

## As abas de Issues e PRs estão vazias

Elas dependem do `gh`, a ferramenta de linha de comando do GitHub. A própria aba diz qual é o caso:
o `gh` não instalado, o `gh` sem login (`gh auth login`), ou o projeto sem um remoto do GitHub. Veja
[o painel do Git](painel-git).

## O app não abre

Depois de travar duas vezes seguidas no arranque, o app sobe numa tela de recuperação, sem carregar
os projetos nem os agentes, oferecendo os backups.

Escolha um ponto na lista e clique em **Restaurar tudo**, **Só as configurações** (quando foi uma
preferência que quebrou o app) ou **Só os projetos**. O estado atual é guardado antes de restaurar.
Sem backup nenhum na lista, resta abrir mesmo assim, e o app tenta começar do zero.

A mesma tela está em **Configurações → Backup**, em **Restaurar de um backup…**, junto de **Fazer
backup agora** e da frequência das cópias.

## Alguma coisa ficou estranha depois que eu mexi nos ajustes

**Restaurar padrões**, no rodapé da barra lateral das Configurações. Ele pede confirmação e devolve
ao original a fonte, a escala, a largura máxima, os atalhos, a voz e os painéis de subagente, além
de desafixar a versão do Claude Code. Não são afetados: a sua chave da OpenAI, os dispositivos de
áudio e os temas dos canvases.

## O instalador aparece como danificado

O download veio incompleto. Baixe de novo. Veja [instalar](instalar).

## Reportar um problema

- **O número da versão** fica no pé da barra lateral das Configurações.
- **O diário da voz** registra cada conexão, queda e reconexão. Os botões **Mostrar no Finder** e
  **Abrir** estão em **Configurações → Diagnóstico**, e ele grava sempre.
- **Os relatórios de queda** do macOS podem ser enviados pelo interruptor **Enviar relatórios de
  queda e de falha de retomada**, no mesmo lugar. A lista das quedas registradas fica logo abaixo,
  com um botão **Enviar** em cada uma. Veja [onde ficam meus dados](onde-ficam-meus-dados).
