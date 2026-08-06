---
slug: a-nina-por-texto
titulo: A Nina por texto
resumo: A caixa do ⌘J: o que ela mostra, quem pensa por trás dela, e como ditar dentro dela.
area: nina
nivel: basico
---

**⌘J** abre e fecha a caixa de conversa escrita, que flutua sobre o canvas. Os ajustes ficam em
**Configurações → Conversa**.

Ela tem as mesmas ferramentas da [conversa por voz](falar-com-a-nina) e do
[modo comando](o-modo-comando), e responde sobre o projeto que está na sua tela naquele momento. A
lista do que dá para pedir está em [o que ela consegue fazer](o-que-ela-consegue-fazer).

## A caixa

- **O campo**: escreva o pedido e aperte Enter. Vale tudo o que você diria falando: "abre dois
  agentes do Codex", "quem está trabalhando?", "traz o Hermes de volta e manda ele rodar os testes".
- **O indicador de atividade**: enquanto ela trabalha, mostra o nome do que está sendo feito naquele
  instante, e não um progresso genérico.
- **O `×` e o clique fora**: fecham a caixa. O que estava escrito no campo continua lá na próxima
  abertura, e uma resposta que ainda estava vindo continua vindo. Com um ditado em andamento, o
  clique fora só fecha a caixa e não atinge o que está atrás dela.
- **Esc**: fecha a caixa.

A caixa nunca mostra o raciocínio nem o resultado bruto das ferramentas.

## O que aparece na caixa

No menu `···`, três modos:

- **Só o campo**: nada além do campo e do indicador de atividade.
- **Última resposta**: o campo e a última frase dela. É o padrão.
- **Conversa inteira**: o fio completo, o que você mandou e o que ela respondeu.

No mesmo menu, **Ver a conversa inteira** abre o histórico numa janela à parte.

## Quem pensa

- **Cérebro da conversa escrita**: escolhe qual CLI de agente responde quando você escreve para ela.
  Roda na assinatura que você já tem, e nunca na OpenAI. O ajuste só aparece com mais de um provedor
  ligado em Configurações → Provedores.

Diferente da conversa por voz, esta continua de onde parou: fechar o app e voltar depois mantém a
mesma conversa.

## Ditar dentro dela

Com a caixa aberta, **⌥D** dita para o campo em vez de mandar para um agente. O cabeçalho passa a
mostrar que está ouvindo, e o fio que normalmente aponta para o agente destinatário não aparece.

- **Ditado envia direto na conversa escrita**: com ele ligado, soltar a tecla já envia. Desligado, o
  texto fica no campo para você conferir e apertar Enter. O padrão é preencher sem enviar. O mesmo
  interruptor está no menu `···` da caixa, com o nome "Enviar ao terminar de ditar".

Apertar ⌥D num canvas sem destino para o texto, seja porque não há agente, seja porque há vários e
nenhum selecionado, **abre a caixa sozinha** antes da primeira palavra.

## A resposta falada

- **Ler a resposta escrita em voz alta**: o app fala a resposta dela com a voz escolhida em
  Configurações → Voz. Desligado por padrão. Em [modo reunião](agenda-e-reunioes) ele continua
  calado.

## O que ela não faz

- Não abre o microfone por conta própria: a voz de entrada é o ditado, e a de saída é opcional.
- Não lê arquivo, não escreve arquivo e não roda comando. Trabalho de código ela entrega a um agente.
- Não é a conversa com um agente. Falar com um agente específico continua sendo o painel dele, ou o
  ditado. Veja [falar com eles](falar-com-eles).
