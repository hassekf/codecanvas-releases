---
slug: painel-custos-e-desempenho
titulo: Uso e desempenho
resumo: Dois painéis: quanto da assinatura de cada provedor já foi e quanto cada agente custou, e quanta memória e CPU o app está usando, por processo.
area: paineis
nivel: basico
---

O painel de uso abre pelo `⌘K` (digite "uso", "consumo" ou "limite"); o de desempenho, por
"desempenho", "cpu" ou "memória".

## O painel de uso

Um bloco por provedor com limite conhecido. Em cada bloco:

- **As janelas de limite** da assinatura, cada uma com a porcentagem já gasta e quando ela zera. O
  anel maior repete a janela mais apertada, que é a que para o trabalho primeiro.
- **O plano**, quando o provedor informa qual é.
- **Os créditos**, quando existem: o quanto foi usado e o teto, na moeda da conta. Eles continuam
  valendo depois que uma janela estoura.
- **visto**: quando aquele número foi lido pela última vez. Provedores que só publicam o consumo ao
  rodar uma sessão podem estar mostrando um número de dias atrás.

Abaixo dos blocos, uma linha apagada com um **travessão** lista os provedores cujo consumo não dá
para ler: Gemini, Cursor e Grok. O travessão quer dizer "não sei", e não zero.

### Neste canvas

Em **NESTE CANVAS**: o total gasto pelos agentes deste canvas, e uma linha por agente com o nome que
você deu a ele. A barra de cada um é proporcional ao maior gasto do canvas, não a um valor absoluto.

O valor é **estimado**: o preço não vem da conversa, vem de uma tabela de preços embutida.

### Contas separadas contam separado

Um limite é da conta, não do projeto. Com mais de uma conta do mesmo provedor em uso, cada uma ganha
o próprio bloco, rotulado com o nome da conta. O consumo de um canvas conta contra a mesma conta em
todos os outros. Veja [contas e perfis](contas-e-perfis).

### As cápsulas do rodapé

Uma cápsula por provedor em uso, com duas metades clicáveis:

- **O logo do provedor**: muda de aparência conforme o serviço está no ar ou com incidente. Clicar
  abre a página de status daquele provedor num painel de navegador aqui dentro.
- **O anel com a porcentagem**: a janela mais apertada daquela conta. Clicar abre o painel de uso.

Com mais de uma conta à mostra, a inicial do nome da conta aparece antes do anel.

O que a assistente e a voz gastam é outra conta, e está em [quanto custa](quanto-custa).

## O painel de desempenho

Ele mede o app, os agentes, os servidores que os agentes sobem e os navegadores, mesmo com o painel
fechado.

- **MEMÓRIA** e **CPU DA MÁQUINA**: os dois números de agora, com o gráfico dos minutos anteriores.
- **A linha abaixo dos números** compara com o normal: ou **no normal deste app**, ou quantas vezes
  o normal o app está pesando agora. É o desvio, e não o número, que dispara um relatório.
- **ONDE ESTÁ A MEMÓRIA**: a divisão por papel, entre **O app**, **Agentes**, **Servidores dos
  agentes**, **Browsers** e **Terminais**.
- **QUEM ESTÁ PUXANDO**: os seis processos mais pesados, com o nome do painel a que cada um
  pertence.
- **Gravar relatório**: escreve agora um relatório com tudo o que está acontecendo e o abre num
  painel.

Quando o sistema não deixa identificar quais processos do WebKit são do app, o painel avisa que os
navegadores **não** estão entrando na conta.

### O número na barra

Ao lado do zoom fica a memória em uso, e a porcentagem de CPU quando ela passa de 10%. Ele ganha cor
ao se aproximar do seu limiar de pico. Clicar abre o painel de desempenho. Ele some com o monitor
desligado.

### O que conta como pico

Em **Configurações → Desempenho**.

- **Medir e gravar relatórios de pico**: liga o monitor. Desligado, nada é medido, nenhum relatório
  é gravado, o painel mostra um botão para religá-lo e o número some da barra.
- **Sensibilidade**: de +10% a +200% acima do que o app costuma pesar. A tela traduz a porcentagem
  para o número de hoje ("aviso acima de X"), e o normal é aprendido em cerca de um minuto de app
  aberto.
- **Abrir a pasta** e **Ver o último**: a pasta dos relatórios, e o relatório mais recente num
  painel.

Cada pico vira um arquivo com os processos, os agentes, o que estava aberto e os minutos anteriores.
Os 30 mais recentes são mantidos, e nenhum deles sai da sua máquina.
