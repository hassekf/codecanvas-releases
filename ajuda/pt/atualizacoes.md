---
slug: atualizacoes
titulo: Atualizações
resumo: A checagem automática, o botão de buscar agora, o que acontece com os agentes na hora de instalar, e as novidades de cada versão.
area: conta
nivel: basico
---

O app procura versão nova sozinho, em segundo plano, a cada hora, e no arranque quando já passou
desse intervalo desde a última vez.

## Pedir na hora

Duas portas, e as duas fazem a mesma coisa:

- **O menu do app → Buscar Atualizações…**
- **Buscar atualizações**, no rodapé das Configurações, ao lado do número da versão. Ele fecha as
  Configurações antes de checar, e fica indisponível enquanto uma checagem está em curso.

A checagem que você pede responde mesmo quando não há nada novo. A automática é silenciosa.

## Os agentes que estão trabalhando

- **A checagem automática não oferece atualização enquanto houver um agente trabalhando.** Ela não
  insiste e não baixa nada: a próxima checagem procura de novo e oferece a versão mais recente de
  então.
- **A checagem que você pede segue mesmo assim.** Ao mandar instalar com alguém trabalhando, o app
  lista pelo nome quem vai ser encerrado e oferece **Adiar** ou **Instalar mesmo assim**.
- **Adiar deixa a atualização baixada esperando.** Enquanto ela não for instalada, é ela que volta a
  ser oferecida, e versões mais novas não aparecem.
- A sessão de cada agente fica salva e você pode chamá-los de volta pelo nome. O que eles estiverem
  fazendo no instante da instalação se perde.

## As novidades

- **Novidades**, no rodapé da tela inicial: abre o que mudou, versão a versão, com a sua marcada.
- **O ponto ao lado do botão**: acende quando há uma versão que você ainda não leu, e apaga quando
  você abre a lista.

A lista é escrita para quem usa o app. A parte técnica de cada versão fica de fora dela.

## Por que dá para confiar no que ele baixa

Cada atualização é assinada, e o app recusa qualquer arquivo cuja assinatura não bata com a chave que
ele carrega. Além disso, o binário baixado continua passando pela conferência da Apple, que é o que
faz o app abrir sem aviso de desenvolvedor não identificado. Veja [instalar](instalar).

## Quando não atualiza

Na ordem em que costuma ser:

1. **Sem internet, ou uma rede que bloqueia o acesso.** Peça pelo botão para ver a resposta.
2. **Há sempre alguém trabalhando.** Use o botão e instale quando puder encerrar os agentes.
3. **Uma atualização adiada, esperando.** Instale-a, e as próximas voltam a chegar.
4. **Nada disso.** Baixe o app de novo e instale por cima. Os canvases, as conversas e as
   configurações não moram dentro do app: veja [onde ficam meus dados](onde-ficam-meus-dados).
