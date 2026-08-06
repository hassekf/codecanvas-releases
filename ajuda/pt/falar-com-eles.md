---
slug: falar-com-eles
titulo: Falar com os agentes
resumo: Mandar tarefa digitando, ditando ou falando, responder o que eles perguntam, destacar um painel e mandar continuar quem caiu.
area: agentes
nivel: basico
---

## Digitando

Clique no painel e escreva. É o terminal do próprio CLI, então os comandos de barra dele e a edição
de linha funcionam ali dentro.

## Ditando

O ditado entrega o texto ao **agente selecionado**, sem passar pela assistente. Sem nenhum painel
selecionado não há destino, e a barra do ditado diz isso. Veja [ditado](ditado).

## Por voz

*"Manda o Hermes rodar os testes"*, *"pergunta pro Atlas se aquilo compilou"*.

- **O texto vai como você falou**, sem paráfrase.
- **Um agente guardado é trazido de volta** com a conversa inteira, em vez de nascer de novo.
- **Dois nomes parecidos param o envio**: o app pergunta qual dos dois antes de mandar qualquer
  coisa.
- **Um verbo do app não vira tarefa**: *"fecha o Perseu"* fecha o painel dele em vez de mandar a
  palavra para dentro do terminal.

## Responder o que eles perguntam

Em **Configurações → Conversa**:

- **Responder os agentes por voz**: depois de avisar em voz alta que um agente espera, o app abre o
  microfone para você responder sem tocar em nada. Desligado, ele continua avisando e deixa a
  notificação mais tempo na tela, sem abrir o microfone.
- **Janela de resposta**: quantos segundos o microfone fica aberto depois do aviso, de 0 a 15, em 6
  por padrão. Em 0 a escuta fica desligada. O controle exige a voz ligada e o interruptor acima
  ligado, e a escuta acontece no seu Mac, sem custo por segundo.

O que é lido, e como responder escolhendo uma opção, está em
[saber o que fazem](saber-o-que-fazem).

## Destacar um painel

*"Foco no Hermes"* põe o painel dele grande à esquerda e reorganiza os outros à direita. Vale para
qualquer painel, e os que não têm nome próprio se chamam pelo tipo: *"foco no browser"*. *"Desfoca"*
devolve todos à grade.

## Mandar continuar quem caiu

*"Manda o Apolo continuar"* é um pedido próprio, diferente de escrever "continue" no terminal: a
mensagem enviada conta o que houve e pede que ele confira o que ficou pela metade antes de refazer
qualquer coisa.

- **Ele respeita a espera entre tentativas**: pedido durante a espera, o app diz em quantos segundos
  vai mandar.
- ***"Quando o Claude voltar"*** põe o agente na fila e só retoma quando o provedor sair da
  instabilidade.
- ***"Deixa quieto"*** cancela a retomada automática daquele agente.

Veja [criar e fechar](criar-e-fechar).

## O histórico do que ele entregou

Em **Configurações → Agentes**, **Histórico de entregas do agente** vem ligado: cada assunto que o
agente conclui vira uma linha no verso do painel dele quando ele passa ao assunto seguinte.
Desligado, o verso mostra só o que ele faz agora.

## Comandos que não terminam

Em **Configurações → Agentes**, **Dev servers em painel próprio** vem desligado. Ligado, comandos
longos como um servidor de desenvolvimento ou um observador de arquivos são abertos num painel de
terminal visível, onde você vê o log e pode interrompê-los. A classificação de comandos longos erra
às vezes.

## Mandar entregar o trabalho

Com os agentes isolados em worktrees, a barra de frentes traz um botão de entrega por frente. Ele não
integra nada: manda o recado ao agente que está dentro daquela cópia do projeto.

Em **Configurações → Interface**, na seção **Barra de frentes**:

- **Como entregar uma frente pronta**: o que o recado pede. **Deduzir de cada destino** é o padrão e
  olha como o trabalho costuma entrar naquele branch; **Merge direto**, **Pull request** e **Só
  avisar** valem para todos os destinos de todos os projetos. A escolha feita no menu da própria
  barra manda por cima, e só naquele destino.
- **Editar o recado**: o texto enviado ao agente. Ele tem três marcadores, que viram o nome da
  branch, o destino e o verbo do modo escolhido. Sem o marcador do verbo, o recado não diz o que
  fazer.

Veja [worktrees e isolamento](worktrees-e-isolamento).

## Falar com um agente é diferente de um agente falar com outro

Um agente conversa com quem ele mesmo trouxe para o canvas, e devolve o resultado a quem o trouxe.
Veja [um agente chama outro](um-agente-chama-outro).
