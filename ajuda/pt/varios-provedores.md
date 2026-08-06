---
slug: varios-provedores
titulo: Vários CLIs de agente
resumo: Claude Code, Codex, Grok e opencode no mesmo canvas: como ligá-los, o que funciona igual em todos e o que é de um só.
area: agentes
nivel: basico
---

Em **Configurações → Provedores**, **CLIs de agente** tem uma linha por CLI: Claude Code, Codex, Grok
e opencode.

- **O estado da linha**: **instalado**, com o nome do executável ao lado, ou **não encontrado no
  PATH**. O app procura cada um no `PATH` do seu shell.
- **O interruptor**: liga o CLI. Um CLI que não está instalado e não está ligado não pode ser
  ligado, e desligar o último ligado não tem efeito.
- **O comando de instalação**: aparece na linha de quem não foi encontrado, com um botão que o copia.
  O app não instala nem atualiza CLI de terceiro. A exceção é o Claude Code, que o painel de um
  agente oferece instalar em um clique quando ele falta.

Um CLI ligado passa a aparecer nos três lugares onde um agente nasce: no `⌘K` (**Novo agente ·
Codex**, **· Grok**, **· opencode**), na barra de comando e na voz, que aceita as grafias que a
transcrição produz para os nomes deles.

## O que é igual em todos

- O painel com o terminal do CLI, e o nome dele no cabeçalho, ao lado do nome do agente.
- Os estados de cada painel e os avisos: trabalhando, esperando você, pronto, caiu, encerrado.
- O verso do painel, com o assunto que o agente escreve sobre si e o histórico de entregas.
- A autoria por arquivo, antes do commit. Veja [o painel do Git](painel-git).
- Dispensar e chamar de volta com a conversa. Veja [criar e fechar](criar-e-fechar).
- As ferramentas do canvas: o navegador próprio, abrir painéis, ler o que outro agente está fazendo e
  trazer colegas.

## O que é de um CLI só

- **Escolher a opção de uma pergunta falando** vale para as perguntas de múltipla escolha do Claude
  Code. Nos outros, a pergunta é lida do mesmo jeito e a resposta vai como texto, digitado ou ditado.
- **Instalar e fixar a versão** é do Claude Code. O menu **Versão do Claude Code**, em
  **Configurações → Agentes**, fixa uma das versões presentes na máquina e, enquanto estiver fixada,
  desliga a atualização automática.
- **Cadastrar instalações** pede uma pasta `.claude`, em **Instalações do Claude**, na mesma tela. Um
  agente escolhe entre elas na criação e no menu de contexto do painel. Ver
  [contas e perfis](contas-e-perfis).
- **O modelo do opencode se escolhe dentro dele**: os modelos que ele roda dependem das contas em que
  você fez login, e o canvas não passa modelo nenhum para ele. Nos outros, o modelo padrão do canvas
  se escolhe em [ajustes do projeto](ajustes-projeto).

## Trocar o CLI de um agente

O menu de contexto do painel não troca o CLI de um agente existente: cada agente vive no CLI em que
nasceu, inclusive quando é chamado de volta depois de dispensado. O que o menu oferece é trocar a
**conta** dele, dentro do mesmo CLI.
