---
slug: busca-e-comandos
titulo: A busca do canvas
resumo: O ⌘K: ir a um painel aberto, criar o que ainda não existe, chamar um agente de volta e abrir um endereço.
area: canvas
nivel: basico
---

Abre com **⌘K**, e a tecla vale mesmo com o cursor dentro de um agente. Ela se troca em
**Configurações → Atalhos**, em "Paleta de comandos".

## As seções do resultado

Os resultados vêm agrupados, e o grupo diz o que o Enter vai fazer.

- **Ir para**: leva a câmera até um painel que já está aberto. Enxerga os painéis de todas as áreas
  de trabalho, e escolher um de outra área troca de área junto. Painel minimizado não entra.
- **Abrir**: cria um painel novo, a partir do catálogo. Só aparecem os agentes dos CLIs ligados em
  **Configurações → Provedores**.
- **Chamar de volta**: recria um agente que você dispensou neste projeto, com a conversa dele.
- **Ação**: o que a sua frase pede e não nomeia. Organizar os painéis, criar uma área de trabalho,
  voltar a um arranjo guardado, abrir um endereço.

Com o campo vazio, a lista traz só a seção **Abrir**, ordenada pelo que você mais abriu por aqui.

## O que mais ela encontra

- **As áreas de trabalho**, pelo nome. Escolher uma troca de área.
- **As suas notas** deste projeto, pelo título. Elas só aparecem quando procuradas.
- **Os arranjos guardados**, pelo nome que você deu. Veja [arrumar o canvas](organizar-sozinho).
- **As execuções em curso** de uma iniciativa, pelo nome da execução. As encerradas não entram.

## O endereço digitado

Uma URL completa abre como está. `github.com` vira `https://github.com`. `localhost:3000` e
`127.0.0.1` abrem em `http://`. Um número sozinho entre 1024 e 65535 abre `http://localhost:<número>`.

Um nome de arquivo não vira endereço: `package.json` não abre no navegador.

## Como o resultado é escolhido

- **Todo termo digitado precisa casar.** "browser mídia" não devolve os dois painéis, devolve nada.
- **O verbo decide entre criar e ir.** "novo navegador" cria um; "vai pro navegador" leva ao que já
  existe. Sem verbo, um painel aberto vem antes de um painel a criar.
- **A grafia errada é aceita** a partir de quatro letras, e sempre abaixo de qualquer casamento
  exato. "brwoser" acha o navegador.
- **O que você mais usa só desempata**, entre dois resultados de mesma pontuação.
- **A etiqueta ao lado do nome mostra o termo que casou**, quando não foi o título que casou.

## Teclado

- **↑ ↓**: andam na lista sem tirar o cursor do campo, e dão a volta no fim.
- **Enter**: abre o resultado selecionado.
- **Esc**: fecha.

## O lembrete no topo do canvas

A pílula no alto do canvas mostra a tecla e não recebe clique. Ela se desliga em
**Configurações → Interface**, em "Lembrete do atalho de busca"; desligada, o topo fica só com as
abas das áreas. O texto dela acompanha o atalho que estiver configurado.

## A busca das Configurações

O campo **Buscar um ajuste**, no alto da barra lateral das Configurações, usa o mesmo motor. Ele
procura no título de cada ajuste, na explicação embaixo dele e nas teclas do app, e aceita termos que
não estão escritos na tela ("dark mode" leva à Interface, "mic" ao microfone).

O resultado escolhido não filtra a tela: ele abre a seção, rola até o ajuste e o acende por alguns
segundos. **↑ ↓** andam na lista, **Enter** salta. **Esc** limpa o campo, e só fecha as Configurações
quando o campo já está vazio.

## O que ela não encontra

Ela não procura dentro dos seus arquivos nem dentro do que os agentes escreveram. Para isso, peça a
um agente.
