---
slug: ajustes-navegador
titulo: Página inicial do navegador
resumo: Em que endereço um navegador novo abre neste projeto, e quando essa escolha não vale.
area: projeto
nivel: basico
---

Em **Editar "nome do projeto"… → Navegador**. A aba tem um controle: **Página inicial**.

## O campo

- **O que ele aceita**: o endereço como uma pessoa o digita. `github.com` vira `https://github.com`,
  `localhost:3000` funciona, e um endereço que já comece com `http://` ou `https://` passa como está.
- **A linha abaixo do campo** mostra em que endereço aquilo vai abrir de verdade, e muda enquanto
  você digita, sem precisar salvar.
- **Em branco, abre no Google.**

A escolha é de cada projeto, e nada é gravado até você salvar a folha.

## Quando ela vale

Vale para o navegador que **você** abre, pelo `⌘K` ou pelo catálogo de painéis, e para o que a
assistente de voz abre a seu pedido.

**Não** vale para o navegador que um agente abre para te mostrar alguma coisa: aquele já vem com um
endereço. Veja [o painel do navegador](painel-navegador) e
[o agente vê o navegador](o-agente-ve-o-navegador).

## A outra escolha sobre navegador

Na aba **Agentes** do mesmo projeto há o **Navegador padrão**, com duas opções:

- **Interno**: o agente mostra o que produziu no navegador de dentro do canvas. É o padrão.
- **Externo**: o agente abre no seu navegador do sistema, e só usa o de dentro quando você pedir.

Aquela responde onde o agente mostra; esta responde em que página um navegador vazio abre. O detalhe
está em [ajustes de agentes](ajustes-agentes).
