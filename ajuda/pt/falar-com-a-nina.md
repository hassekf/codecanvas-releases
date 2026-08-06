---
slug: falar-com-a-nina
titulo: Falar com a Nina
resumo: Abrir e encerrar a conversa por voz, o que fecha um turno, os dois relógios e o bom-dia.
area: nina
nivel: basico
---

**⌥C** abre e fecha a conversa por voz. Os ajustes ficam em **Configurações → Conversa**, e o
bom-dia, em **Configurações → Saudação**.

A Nina age no canvas com as mesmas ferramentas do [modo comando](o-modo-comando) e da
[conversa escrita](a-nina-por-texto). O que ela pode fazer está em
[o que ela consegue fazer](o-que-ela-consegue-fazer); os grupos de ferramentas se ligam e desligam em
Configurações → Ferramentas.

## Abrir e encerrar

- **⌥C**: liga e desliga a conversa. É um interruptor, não um segurar e falar.
- **"Pode dormir"**, "tchau", "valeu", "chega": encerra a conversa. Ela não se despede; o silêncio é a
  confirmação. Os agentes continuam trabalhando.
- **Esc**: corta a conversa e a fala em andamento, com o app em qualquer janela.
- **Confirmar ao ativar**: faz a Nina dizer uma palavra quando o microfone abre. Desligado, a
  primeira coisa da conversa é a sua voz.
- **Palavra de abertura**: troca essa palavra. Em branco, vale a palavra padrão do idioma ativo.

Quando a conversa é acordada por um aviso, ela não diz a palavra de abertura e já entra sabendo de
qual agente se trata.

A conversa por voz não guarda nada de uma sessão para a outra: encerrada, a próxima começa sem o que
foi dito antes. Quem guarda memória são os agentes, e [a conversa escrita](a-nina-por-texto).

## Durante a conversa

- Começar a falar interrompe a Nina no meio da frase.
- O turno fecha por **silêncio**, nunca por tamanho da fala. Quanto silêncio conta como fim é o
  **Silêncio para ela responder** (padrão 900 ms), e de que volume para cima o som conta como voz é a
  **Sensibilidade do microfone**, os dois em Configurações → Conversa.
- A moldura da janela acende enquanto ela fala.
- Enquanto a conversa está no ar, o painel de mídia é silenciado.
- A conversa não abre em [modo reunião](agenda-e-reunioes): ⌥C mostra uma notificação dizendo que o
  microfone está com a chamada, com o botão de sair junto.

### Os dois relógios

- **Encerrar após silêncio**: encerra a conversa depois desse tempo sem ninguém falar. De 0 a 300
  segundos, padrão 90. Zero desliga.
- **Tempo máximo da conversa**: encerra ao fim do tempo mesmo com você falando, e é o único que
  garante um teto de gasto. De 0 a 30 minutos, padrão 5. Zero é sem teto. No último minuto a
  janelinha da voz mostra a contagem regressiva.

## Quando o app fala primeiro

Um agente que termina, que pergunta ou que cai gera um aviso, e o app o fala se houver alguma voz
ligada. Quais eventos avisam, com som e com voz, está em [avisos e sons](avisos-e-sons).

- **Responder os agentes por voz**: depois do aviso falado, o app abre o microfone por alguns
  segundos para você responder falando. Desligado, ele só avisa.
- **Janela de resposta**: quanto tempo essa escuta dura, de 0 a 15 segundos, padrão 6. Zero desliga a
  escuta. Ela usa o reconhecimento local e não gasta créditos.

O que você diz nessa janela decide o que acontece:

- **"Me leva lá"**, "abre o painel dele", o nome do agente: leva você até ele, trocando de projeto e
  de área se for preciso.
- **"Depois"**, "beleza", "deixa pra lá": encerra a escuta sem fazer nada.
- **"Continua"**, "tenta de novo", "pode mandar": manda o agente retomar. Só vale logo depois de um
  aviso de queda.
- **"Só quando voltar ao ar"**: espera o provedor voltar antes de retomar. Só vale logo depois de um
  aviso de queda.
- **Qualquer outra frase**: acorda a conversa, já sabendo de qual agente o aviso falava. Basta uma
  palavra que o app não reconheça para a frase inteira ir para a conversa.

Ficar calado fecha a janela sem gastar nada.

## O bom-dia

Em Configurações → Saudação.

- **Bom-dia ao abrir**: o app conta como está o dia na primeira vez que você o abre no dia, e só
  quando há alguma pendência. Com a Nina ligada, o bom-dia vira conversa; com ela desligada e alguma
  voz ligada, é um recado falado; sem voz nenhuma, é uma notificação na tela.
- **Falar das tarefas**: inclui o que venceu e o que vence hoje nas suas listas.
- **Falar das reuniões**: inclui os compromissos de hoje, se [a agenda](agenda-e-reunioes) estiver
  conectada.

Abaixo dos interruptores, a seção **Hoje** mostra sobre o que ele falaria se você abrisse o app
agora, projeto por projeto. Sem pendência em nenhum projeto, ele não fala.

Os dois interruptores de conteúdo avisam quando o grupo de ferramentas correspondente está desligado
em Configurações → Ferramentas: a Nina menciona a tarefa ou a reunião, mas não consegue mexer nelas
por voz.
