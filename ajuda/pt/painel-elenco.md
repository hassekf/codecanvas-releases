---
slug: painel-elenco
titulo: O painel do elenco
resumo: A lista dos agentes deste projeto em quatro seções, o que a busca alcança, e o que cada botão faz com um agente guardado.
area: paineis
nivel: basico
---

Os agentes deste projeto numa lista, os que estão na tela e os que já foram dispensados. Abra pelo
`⌘K` digitando "elenco". O painel é um por canvas.

A lista é do projeto: cada canvas tem o seu elenco. Os agentes que rodam os passos de uma
[Iniciativa](painel-iniciativas) não entram aqui.

## As quatro seções

Cada uma traz a contagem no cabeçalho.

- **Na tela**: os agentes abertos e acordados, com o sinal de estado e o que cada um está fazendo.
- **Hibernando**: os agentes abertos que dormiram por inatividade. Continuam no canvas e acordam ao
  receber um prompt. Quem controla isso é **Hibernar agentes inativos**, em
  [configurações dos agentes](ajustes-agentes).
- **Guardados**: os agentes dispensados que têm conversa para retomar, com a última missão entre
  aspas e há quanto tempo estiveram ativos.
- **Guardados sem histórico**: os dispensados que nunca receberam uma tarefa. Só ocupam um nome.

Sem nenhum agente, o painel diz que o projeto ainda não tem nenhum; com a busca preenchida e sem
resultado, diz que nada foi encontrado.

## A busca

O campo no topo filtra as quatro seções ao mesmo tempo. Ele olha o nome, a missão, o assunto e o
resumo que o agente anotou, a pendência dele, e **todas as entregas** que ele registrou, inclusive
as dos agentes já dispensados.

Quando o que casou com a busca foi uma entrega antiga, essa entrega aparece na própria linha, com há
quanto tempo foi. A mesma busca funciona por voz: *"quem trabalhou no pagamento?"*.

## Os botões de cada linha

- **Ir até o painel** (na seção Na tela): seleciona o agente e leva a câmera até ele.
- **Chamar** (nos guardados): reabre o agente com a conversa dele inteira. Ele volta com o mesmo
  nome e o mesmo histórico.
- **Esquecer** (nos guardados, ao passar o mouse na linha): tira o agente do elenco e libera o nome.
  Pede confirmação, e não tem desfazer.
- **Clicar na linha** abre o resumo.

Os guardados também aparecem no `⌘K` quando você digita o nome deles, e escolhê-los ali é o mesmo
que apertar **Chamar**. Eles só aparecem na [busca](busca-e-comandos) quando procurados.

## A linha aberta

- **O que o agente anotou**: o assunto, o resumo e a pendência, quando ele registrou alguma. Sem
  resumo anotado, aparece a missão; sem nenhum dos dois, o painel diz que ele ainda não anotou nada.
- **Entregou**: a linha do tempo do que ele já entregou, da mais recente para a mais antiga, com há
  quanto tempo cada uma foi. Ela mostra as seis últimas e resume o resto numa linha.

Este é o único lugar onde o histórico de um agente **dispensado** aparece. Para acompanhar quem
está na tela, veja [saber o que fazem](saber-o-que-fazem).

## Limpar as seções

- **Esquecer todos**, no cabeçalho de **Guardados**: esquece todos os que têm conversa. Pede
  confirmação duas vezes.
- **Liberar nomes**, no cabeçalho de **Guardados sem histórico**: esquece todos de uma vez, com uma
  confirmação.

Nos dois casos os nomes voltam a ficar livres para agentes novos, e não há mais como chamar de volta
quem foi esquecido.
