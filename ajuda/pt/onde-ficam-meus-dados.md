---
slug: onde-ficam-meus-dados
titulo: Onde ficam os seus dados
resumo: O que o CanvasCode guarda na sua máquina, onde ele guarda os segredos, e o que sai daqui, para onde e a mando de quê.
area: conta
nivel: basico
---

O CanvasCode não tem conta e não tem servidor próprio de dados. O que sai da sua máquina sai porque
uma funcionalidade que você usou precisa de um serviço de fora, e esta página diz qual, e o quê.

## No seu disco

Em `~/Library/Application Support/codeCanvas`:

- **`canvases.json`**: os projetos, os painéis com posição e tamanho, as áreas de trabalho, o tema, o
  fundo, os arranjos guardados e o registro dos agentes que já viveram em cada projeto.
- **`tarefas/` e `notas/`**: um arquivo por projeto.
- **`imagens/`**: as imagens geradas e coladas, uma pasta por projeto, com o pedido que criou cada
  imagem gerada.
- **`fundos/`**: cópia de cada papel de parede que você escolheu ou pediu.
- **`modulos/` e `modulos-dados/`**: os módulos que você criou e o que eles guardam.
- **`voz/`**: o extrato de uso da voz, um arquivo por dia, e o diário técnico que registra cada
  conexão do microfone.
- **`custos/`**: o registro do que a voz e a conversa gastaram.
- **`Recados/`**: os recados já abertos, os que você enviou e a fila de confirmação.
- **`entregas/`**: o que um agente escreve para outro quando um deles delega uma tarefa.
- **`backups/`**: cópias automáticas do `canvases.json`, das preferências, das tarefas e das notas.
- **`crashes.json` e `quedas.jsonl`**: o registro das quedas do app e das quedas de agentes.

As **gravações de tela** vão para `~/Movies/codeCanvas`. As **preferências** do app ficam onde o
macOS guarda preferência de app.

Nada disso é enviado a lugar nenhum, e os backups também não saem da máquina.

## Os segredos

Ficam no **Keychain do macOS**, e nunca num arquivo de texto:

- a sua chave da OpenAI;
- a sua chave de licença e o token que a ativação devolve;
- os tokens das integrações que você conectar, um por projeto;
- os segredos que você cadastrar nos servidores MCP;
- as chaves privadas deste Mac para os recados.

O campo da chave da OpenAI mostra se ela está configurada, e nunca a chave. Os backups não levam
nenhum destes itens.

## A conversa dos agentes

Ela é do programa de agente, não do app, e mora na pasta dele: `~/.claude`, `~/.codex` e equivalentes,
ou a pasta da conta que você escolheu para aquele projeto. O CanvasCode guarda apenas a **chave** de
cada conversa, que é o que permite chamar um agente de volta com a memória inteira.

Um agente chamado de volta noutra conta não encontra a conversa que teve na primeira. Veja
[contas e perfis](contas-e-perfis).

## O que sai daqui

### Os agentes

O que você manda a um agente vai para o serviço dele, como iria se você rodasse o mesmo programa no
seu terminal. O app não intermedeia essa conversa e não guarda cópia dela.

### A voz, o comando e as imagens

Tudo isto usa a sua chave da OpenAI, e nada disso acontece sem ela.

- **A conversa com a assistente** manda e recebe **áudio**.
- **A voz que ela usa para falar** manda o texto a ser lido.
- **O modo comando** manda **texto**: a frase transcrita, mais os nomes dos agentes vivos, dos
  projetos abertos, dos temas e dos CLIs ligados. Sem chave, ele usa o modelo que roda no seu Mac.
- **Gerar uma imagem** e **pedir um papel de parede** mandam o seu pedido. O "buscar" do papel de
  parede procura na web pelo serviço da OpenAI.

O **ditado** não sai da máquina em nenhum dos dois motores: o do sistema transcreve pelo macOS, e o
Parakeet roda no seu Mac depois de baixar o modelo. Veja [ditado](ditado) e
[quanto custa](quanto-custa).

### A agenda

A agenda só é lida se você a ligar em **Configurações → Integrações**. Ligada, cinco itens de cada
compromisso podem ser mandados à assistente junto da conversa, e você escolhe um a um: título, local,
descrição e pauta, participantes e link da chamada. Todos nascem ligados. Você também escolhe quais
agendas do Calendar entram. Veja [agenda e reuniões](agenda-e-reunioes).

### Os recados

Um recado sai deste Mac cifrado de ponta a ponta, com chaves que só existem no Keychain daqui e no do
destinatário. O servidor entrega e esquece o envelope; a cópia que fica é a do seu disco. Veja
[o painel de recados](painel-recados).

### As integrações de empresa

Jira e Confluence falam com o servidor da sua organização, e só quando você pede. Veja
[Jira e Confluence](jira-e-confluence).

### A licença

Ativar, revalidar e liberar o Mac mandam a sua chave de licença, um **código derivado do
identificador deste Mac**, e o nome do Mac como o macOS o conhece. A ativação manda também a versão
do app e a do macOS. O código do Mac é embaralhado e não é reversível. Veja [licença](licenca).

### Os relatórios de queda

Quando o app trava, o macOS grava um relatório técnico no seu disco. O interruptor **Enviar
relatórios de queda e de falha de retomada**, em **Configurações → Diagnóstico**, decide se ele é
enviado; o app pergunta na primeira vez que houver o que mandar.

- O relatório traz o rastro de onde o app tropeçou, a versão dele e a do macOS. Ele **não** carrega o
  seu código nem os seus arquivos.
- O mesmo interruptor cobre a falha em que um agente volta sem a conversa dele. Aí vão contagens,
  datas e os identificadores das sessões; o caminho do seu projeto vira um código, e o nome das suas
  contas não sai daqui.
- Desligado, nada é enviado. A lista abaixo do interruptor mostra o que já foi recolhido e o que
  ainda está para mandar, com um botão de enviar em cada linha.

### As atualizações

O app consulta o servidor de atualizações para saber se há versão nova e baixa quando há. Cada
atualização é assinada, e o app recusa qualquer arquivo cuja assinatura não confira. Veja
[atualizações](atualizacoes).

## Os agentes falam com o canvas sem sair da máquina

Quando um agente abre um painel, lê as suas tarefas ou fotografa o navegador, ele fala com um
servidor que o app sobe dentro do seu Mac. Ele escuta só em loopback, e exige um segredo que nasce a
cada execução do app e é entregue a cada agente que nasce aqui.

## Levar tudo embora

A pasta do app é uma pasta comum: dá para copiá-la, guardá-la ou apagá-la pelo Finder. Fora dela
ficam os segredos no Keychain, as gravações em `~/Movies/codeCanvas` e as conversas dos agentes, que
são do programa deles.
