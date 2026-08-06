---
slug: saber-o-que-fazem
titulo: Saber o que eles estão fazendo
resumo: O estado de cada painel, o verso com o retrato do agente, os sinais fora da vista e o que dá para perguntar por voz.
area: agentes
nivel: basico
---

## O estado no cabeçalho do painel

O ponto ao lado do nome tem cinco estados:

- **Trabalhando**: o agente recebeu uma tarefa ou está usando alguma ferramenta.
- **Esperando você**: ele parou numa pergunta ou num pedido de permissão. O ponto pulsa.
- **Pronto**: ele terminou e está parado.
- **Caiu**: a resposta foi interrompida por erro da API. Veja [criar e fechar](criar-e-fechar).
- **Encerrado**: o processo dele saiu.

O estado continua correto com o painel minimizado, em outra área de trabalho ou em outro canvas.

## A linha do assunto, no painel

Abaixo do cabeçalho de cada agente fica o assunto que ele escreveu sobre o que está fazendo. O
parágrafo inteiro, e o que ele espera de você, aparecem ao passar o cursor por ela.

- **Duplo clique na linha** escreve um assunto seu, que o agente não reescreve mais. O mesmo está no
  menu de contexto do painel, em **Escrever um assunto…**.
- **Confirmar com o campo vazio**, ou **Devolver ao agente** no menu de contexto, desfaz a fixação.
- O assunto fixado por você não alcança o verso do painel, que continua mostrando o que o agente
  escreveu.

## O verso do painel

**`⌥F`** vira todos os painéis do canvas de uma vez, e `⌥F` de novo desvira. A tecla está em
**Configurações → Atalhos**, como **Ver status**, e a mesma coisa se pede por voz com *"vira os
painéis"* e *"desvira"*.

No verso de um agente:

- **O assunto e o resumo**, escritos pelo próprio agente sobre o que ele está fazendo.
- **O que ele espera de você**, quando espera.
- **A sua última tarefa**, precedida de "você pediu", quando o agente já escreveu um assunto. Sem
  assunto escrito, a tarefa aparece sozinha, entre aspas, e um agente que ainda não recebeu nada
  mostra "Sem missão ainda".
- **O que ele fez**: a contagem de ferramentas desde a tarefa atual, ou o passo em curso enquanto ele
  trabalha.
- **O estado e o tempo**: há quanto tempo ele trabalha, ou há quanto tempo o resultado está ali. No
  estado de queda, esta linha mostra a contagem para a próxima tentativa, ou que o app está
  esperando o provedor voltar.
- **Agora** e **Entregou**, quando o agente já concluiu alguma coisa: duas abas, com a contagem de
  entregas no rótulo da segunda. A trilha lista as entregas da mais recente para a mais antiga, e
  cada linha abre mostrando o resumo daquele momento. Ela se desliga em
  [ajustes dos agentes](ajustes-agentes).

## Quando o agente termina fora da sua vista

- **Brilho no painel ao terminar**, em **Configurações → Interface**: a moldura do painel brilha
  quando o agente entrega, mesmo sem ele estar selecionado.
- **Destacar a aba da área ao terminar**, na mesma tela: a aba da área pisca quando alguém termina ou
  passa a esperar você numa área que você não está vendo.
- **Cor do brilho de conclusão**, também ali, vale para os dois, e o botão **Padrão** desfaz a
  escolha.

## Perguntar em vez de olhar

Com a voz configurada:

- ***"Como estão todos?"***: o assunto de cada agente.
- ***"O que o Hermes está fazendo?"***: a tarefa dele, o que ele fez e o que ele respondeu por
  último.
- ***"Quais agentes eu tenho?"***: os que estão na tela e os guardados, com o assunto e as últimas
  entregas de cada um.
- ***"Quem mexeu no pagamento?"***: procura o assunto no histórico de todos os agentes do projeto,
  inclusive os guardados, e alcança os outros projetos se você pedir.

Veja [o que ela consegue fazer](o-que-ela-consegue-fazer).

## Quando é o agente que pergunta

O app lê a pergunta e as opções em voz alta e aceita a resposta falada: o rótulo da opção, o número
dela, ou uma resposta sua que não está entre as opções. Uma resposta que não casa com opção nenhuma
faz a pergunta ser repetida, em vez de escolhida por aproximação, e com dois agentes perguntando ao
mesmo tempo o app pergunta para qual deles é a resposta.

Escolher a opção falando vale para as perguntas de múltipla escolha do Claude Code. Nos outros CLIs a
resposta vai como texto, digitado ou ditado. Veja [vários provedores](varios-provedores).

## Um agente lendo o outro

Um agente pode ler o que outro agente deste projeto recebeu, fez e disse por último, e não pode
mandar nada para ele. Veja [um agente chama outro](um-agente-chama-outro).

A lista completa, com os que estão na tela e os guardados, está em
[o painel do elenco](painel-elenco).
