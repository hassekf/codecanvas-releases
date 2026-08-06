---
slug: agenda-e-reunioes
titulo: Agenda e reuniões
resumo: Conectar o calendário do Mac, o que a Nina pode ver dele, o aviso antes da hora e o modo reunião.
area: integracoes
nivel: basico
---

Em **Configurações → Integrações**. O CanvasCode lê o Calendário do Mac, com todas as contas que já
estão nele, e nunca escreve nada na sua agenda.

## Conectar

- **Conectar a agenda**: liga a integração. O macOS pede a permissão nesse momento. Negada a
  permissão, o interruptor volta para desligado, e a seção mostra um botão que abre Privacidade e
  Segurança → Calendários nos Ajustes do Sistema, porque o macOS não pergunta de novo sozinho.

Ligada, a seção mostra quantos compromissos há hoje. Desligada, a integração não deixa rastro:
nenhum bloco na tela inicial, nenhum aviso, e a Nina não recebe nada sobre o assunto.

- **Quais agendas entram**: marca e desmarca cada calendário do Mac. Nenhuma marcada quer dizer
  todas.

## O que a Nina pode ver

Cinco itens, ligados por padrão, que decidem o que sobe para a OpenAI quando você pergunta à Nina
sobre a agenda:

- **Título**: sem ele, ela só sabe que existe um compromisso.
- **Local**: a sala, o endereço, o prédio.
- **Descrição e pauta**: o corpo do convite.
- **Participantes**: quem foi convidado e quem confirmou.
- **Link da chamada**: o endereço do Meet, Zoom ou Teams. Sem ele, ela não consegue abrir a chamada
  por voz.

O horário sempre acompanha o compromisso, marque você o que marcar. Os avisos, o bloco do dia e as
notificações na tela são montados no seu Mac e não passam pela OpenAI, independente destes cinco.

O grupo inteiro de ferramentas de agenda também se desliga em Configurações → Ferramentas: aí a Nina
deixa de ler o calendário e de entrar em chamada, e a integração continua conectada.

## O seu dia na tela inicial

Abaixo dos projetos aparece um bloco com os compromissos de hoje, ou os de amanhã quando hoje já não
tem nenhum. O cabeçalho diz qual dos dois dias está sendo mostrado.

- O que já passou fica na lista, apagado; o que está acontecendo aparece marcado como "agora".
- Passar o mouse numa reunião com link mostra o botão **Entrar**.
- Clicar na linha abre o detalhe: horário, agenda de origem, participantes, pauta e um botão
  **Abrir no Calendário**, que é onde se cria, se move e se cancela compromisso.

## O aviso antes da hora

- **Avisar antes da reunião**: mostra uma notificação antes de a reunião começar. Ela não some
  sozinha.
- **Avisar antes**: quantos minutos antes, entre 5, 10, 15 e 30. O padrão é 10.

O aviso é de uma reunião por vez, sempre a próxima que ainda não começou. Numa reunião com link ele
traz os dois caminhos de entrada, o da sua preferência na frente e o outro logo ao lado, mais o botão
**Depois**, que o dispensa. O aviso sai sozinho uma hora depois do fim da reunião, ou no instante em
que ela for cancelada no calendário.

- **Ao abrir uma reunião**: escolhe entre "Num painel daqui" e "No meu navegador". Aqui dentro, o
  Meet abre com a sessão do Google que os painéis de navegador já usam.

Ao entrar por um painel daqui, a chamada vira o assunto da tela quando o canvas se organiza sozinho.
Com os painéis arrumados à mão, nada é movido de lugar.

## O modo reunião

Entrar numa chamada pelo aviso, pela voz ou pelo botão liga o modo reunião. Com ele ligado:

- Nada é falado e nenhuma notificação aparece.
- O microfone não abre sozinho depois de um aviso.
- **As teclas de ditado, comando e conversa não abrem o microfone.** Apertar uma delas mostra uma
  notificação dizendo que o microfone está com a sua reunião, com o botão de sair junto.
- A conversa por voz que estivesse aberta é encerrada ao entrar.

O selo na barra mostra "Em reunião" e serve de saída: clicar nele desliga o modo. O modo também sai
sozinho cinco minutos depois do fim do compromisso, e sai quando você fecha o painel em que a chamada
tinha aberto.

Pela voz, "fica quieta um pouco" liga o modo sem reunião nenhuma, e "acabou a reunião" o desliga.

### Nada se perde

O que chegaria durante a reunião fica guardado. Ao sair, os avisos que descrevem um problema ainda
vivo, como um agente caído, voltam inteiros; os demais viram uma notificação dizendo quantos
chegaram, com um botão **Ver** que abre o histórico.

## Por voz

```
"o que eu tenho hoje?"           "qual a próxima reunião?"
"do que é a reunião das três?"   "quem vai estar nela?"
"entra na reunião"               "abre o Meet"
"fica quieta um pouco"           "acabou a reunião"
```

Sem dizer qual, ela entra na que está acontecendo ou na próxima a começar. Não há como criar, mover
ou cancelar compromisso por voz.

## No bom-dia

- **Falar das reuniões** (Configurações → Saudação): inclui os compromissos de hoje na saudação da
  manhã, na mesma frase das outras pendências. Veja [falar com a Nina](falar-com-a-nina).
