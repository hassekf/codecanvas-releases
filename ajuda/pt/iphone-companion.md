---
slug: iphone-companion
titulo: O iPhone pareado
resumo: Parear o iPhone com este Mac, revogar um aparelho, o que dá para fazer de longe e quando o telefone avisa.
area: integracoes
nivel: basico
---

Em **Configurações → Companion**. O app do telefone chama-se Canvas Companion, e faz parte do plano
**Team**.

## Parear

- **Parear um iPhone**: abre a janela do convite. Ela traz um QR, para a câmera do telefone, e o
  mesmo convite escrito num código de 6 caracteres, para ditar.
- **Copiar código**: põe o código na área de transferência.
- **O convite vale 5 minutos e uma vez só**, e morre quando você fecha essa janela. Um relógio na tela
  conta o tempo restante.
- **Gerar outro convite**: substitui o convite expirado. Ele não é gerado sozinho.
- Quando o telefone entra, a janela troca o QR pelo nome do aparelho.

Se você pareou digitando o código em vez de ler o QR, confira os caracteres de **Este Mac**
com os que aparecem no telefone. É essa comparação que prova que a chave guardada lá é a deste
computador.

## A lista de aparelhos

Cada linha traz o nome do aparelho, quando ele foi pareado, quando falou com este Mac pela última vez
e a impressão da chave dele.

- **ainda não falou com este Mac**: substitui a data de uso enquanto o telefone não se apresentou.
- **chave trocada em <data>**: aparece quando as chaves daquele aparelho mudaram. Reinstalar o app do
  telefone e alguém tomar a conta chegam aqui do mesmo jeito.
- **Revogar**: este Mac para de aceitar aquele aparelho na hora, sem diálogo de confirmação. Para
  voltar, é preciso parear de novo, com o Mac na frente.
- **Este Mac**: mostra o nome desta máquina e a impressão da chave dela. Trocar de Mac exige parear
  os telefones outra vez.

Sem nenhum aparelho pareado, nada de fora fala com este Mac.

## O que dá para fazer do telefone

- **Ver os projetos e os agentes de cada um**, com o estado de agora, o último pedido que você fez e
  os arquivos que cada um escreveu.
- **Ler a conversa** de um agente, mensagem a mensagem.
- **Abrir um arquivo** que o agente escreveu.
- **Ver o que mudou** na pasta em que o agente trabalha.
- **Responder a pergunta** que parou um agente, escolhendo entre as opções ou escrevendo outra
  resposta.
- **Mandar trabalho** a um agente. O envio normal passa pela fila do app: ele acorda o agente que
  está dormindo, espera uma permissão aberta, e ainda dá para cancelar antes de sair. O envio direto
  escreve no terminal na hora, e o telefone pede um gesto a mais para usá-lo.
- **Interromper** quem está no meio de algo, e **dispensar** quem já acabou.
- **Abrir um projeto** e trocar o projeto em foco aqui no Mac.
- **Chamar um agente novo**, e criar uma área de trabalho.
- **Falar com a Nina**, que responde com o que sabe deste canvas.

Um pedido de ação repetido não executa duas vezes: tocar em "tentar de novo" devolve o resultado do
primeiro.

## Quando o telefone avisa

O telefone toca a campainha em três casos: um agente **parou para perguntar** (o aviso traz o
enunciado da pergunta), um agente **terminou** e um agente **caiu**. O estado de rotina viaja para a
tela sem tocar a campainha.

## Os limites

- **O arquivo tem de estar na pasta em que aquele agente trabalha.** Nada fora dela é alcançável, e
  um arquivo grande chega cortado, com o aviso de que foi cortado.
- **A lista do que o agente escreveu vem das ferramentas de escrita da CLI.** Um arquivo criado por
  um comando de terminal não entra nela.
- **O Mac precisa estar acordado.** Com ele dormindo, o telefone recebe uma resposta dizendo que o
  Mac não está pronto.
- **Cada comando que chega passa pela licença e pela chave do aparelho** antes de virar ação, e o que
  apaga trabalho pede confirmação no próprio telefone.
