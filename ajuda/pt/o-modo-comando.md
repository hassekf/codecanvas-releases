---
slug: o-modo-comando
titulo: O modo comando
resumo: Segurar ⌥X e falar uma ordem: o que ele aceita, o que ele recusa e como a frase vira ação.
area: nina
nivel: basico
---

**⌥X**: segure a tecla, fale a ordem, solte. A tecla se troca em **Configurações → Atalhos**, na
linha "Comandar".

O comando executa e confirma numa frase curta. Ele não abre conversa e não escuta a sua resposta.
Para conversar, use [a Nina por voz](falar-com-a-nina) (⌥C); para escrever um texto dentro de um
agente, use [o ditado](ditado) (⌥D).

## O que dá para mandar

As mesmas ferramentas da Nina, e a lista está em
[o que ela consegue fazer](o-que-ela-consegue-fazer). Exemplos que funcionam como estão:

```
"abre um agente"                      "sobe dois agentes"
"ei Freya, roda os testes"            "pede pro Apolo revisar o login"
"chama a Freya de volta"              "quais agentes existem?"
"quem foi que mexeu no pagamento?"    "como estamos?"
"abre o git"                          "fecha o browser"
"coloca o browser em foco"            "me leva até a Gerda"
"anota aí que eu preciso arrumar o login"
"organiza as janelas uma embaixo da outra"
"troca o tema pra forja"              "põe um fundo de floresta"
```

### Várias ordens numa frase

Uma frase pode carregar quantas ordens você disser, e elas são executadas na ordem em que aparecem:

```
"fecha o Apolo e organiza em duas colunas"
"bom dia! fecha a Gerda, abre dois agentes, põe em duas colunas e mostra o status"
```

Cumprimentos não contam como ordem, e a mesma ordem dita de dois jeitos ("minimiza o vídeo, quero só
o áudio") continua sendo uma.

### Quando não há ordem nenhuma

Frases como "testando, você está me ouvindo?" ou "olá, tudo bem?" recebem uma resposta curta e nada
acontece na tela. Não entender e não haver ordem são coisas diferentes: no segundo caso o app
responde em uma frase, em vez de inventar uma ação.

## O que ele recusa

Toda ordem passa por uma verificação antes de ser executada, e quatro coisas são impossíveis:

- **Fechar sem um verbo de fechar na sua frase** ("fecha", "tira", "apaga", "dispensa", "limpa").
- **Fechar tudo sem a palavra "tudo"**.
- **Criar um agente sem um verbo de criação**. Dizer a palavra "agente" não basta: "põe os agentes em
  três colunas" não cria ninguém.
- **Mandar qualquer coisa para um agente cujo nome você não pronunciou.**

Quando uma dessas travas barra alguma coisa, o motivo fica registrado no diário da voz, em
Configurações → Diagnóstico.

## Como a frase vira ação

A sua fala é transcrita no próprio Mac, e só o texto sai daqui. Quem interpreta o texto é o modelo
escolhido em **Configurações → Voz → Modelo do comando**, que depende da chave da OpenAI. Sem chave,
sem rede ou com o pedido sem resposta, um modelo do próprio Mac assume, e depois dele um roteador de
palavras-chave.

O modo comando custa uma fração de um turno de conversa. Ver
[quanto custa](quanto-custa).

## O que você vê e ouve

- Enquanto a tecla está pressionada, uma janelinha mostra o texto sendo transcrito.
- Quando a ordem vai para um agente, uma faísca cruza o canvas até o painel dele, mostrando para
  quem o app mandou.
- A confirmação é falada com a voz natural, ou com a do sistema quando ela está desligada. A voz
  começa cerca de um segundo depois; a ação já aconteceu antes disso.
- **Esc** cancela o comando em andamento.

## O idioma

**O comando de voz entende português.** A interface do CanvasCode fala português, inglês e espanhol,
e [o ditado](ditado) acompanha o idioma escolhido, mas as ordens faladas são interpretadas em
português. Uma ordem dita em outra língua não é executada.
