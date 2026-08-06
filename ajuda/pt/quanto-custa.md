---
slug: quanto-custa
titulo: Quanto custa a voz
resumo: O que usa créditos da OpenAI, o que pesa na conta da conversa, os dois tetos e onde ver o gasto.
area: nina
nivel: basico
---

Em **Configurações → Custos**. O gasto sai dos créditos pré-pagos da conta de API cuja chave você
salvou em [Configurações → Conversa](configurar-a-voz). Assinatura do ChatGPT não dá acesso à API.

## O que não usa créditos

- **O ditado**: a transcrição acontece no seu Mac. Veja [ditado](ditado).
- **A voz do sistema**: é a voz do macOS, e é ela que fala quando a voz natural está desligada.
- **A escuta que abre depois de um aviso falado**: usa o reconhecimento local. Ficar calado nela não
  gasta nada.
- **[A conversa escrita](a-nina-por-texto)** (⌘J): responde com o CLI de agente que você já assina.

## O que usa créditos

- **A conversa por voz** (⌥C): áudio de ida e de volta. É o item mais caro.
- **[O modo comando](o-modo-comando)** (⌥X): só texto, porque a transcrição é feita no seu Mac.
- **A voz natural**: os avisos falados e as confirmações do comando.
- **O bom-dia**: a frase é escrita por um modelo quando há chave; sem chave, o app monta a frase
  sozinho e não gasta nada.
- **A geração de imagem e o papel de parede pedido por voz**. A qualidade escolhida muda bastante o
  preço. Veja [a galeria](painel-galeria).

## O que pesa na conta da conversa

- **O áudio que ela fala** é o item mais caro de todos, e nunca é reaproveitado.
- **Cada resposta reprocessa a sessão inteira**: as instruções, as ferramentas e o histórico. A conta
  sobe com a duração da conversa, não com o volume da sua voz.
- **As ferramentas ligadas entram nesse reprocessamento.** Em **Configurações → Ferramentas**, o
  bloco do topo mostra o custo aproximado de cada troca com a seleção atual, e quantas trocas por
  minuto cabem no limite da sua conta; cada grupo mostra quanto custa. Desligar um grupo tira as
  ferramentas dele da conversa e não desfaz a integração.

## Os dois tetos

Em Configurações → Conversa.

- **Encerrar após silêncio**: encerra depois desse tempo sem ninguém falar. Padrão 90 segundos, zero
  desliga.
- **Tempo máximo da conversa**: encerra ao fim do tempo mesmo com você falando, e é o único que
  garante um limite de gasto por conversa. Padrão 5 minutos, zero é sem teto.

## O modelo

- **Modelo da Nina**: o modelo da conversa por voz, e o preço muda com ele. A lista vem da sua conta,
  e o botão "Atualizar" a refaz. O app escolhe o primeiro da lista quando o modelo guardado deixa de
  estar disponível.
- **Modelo do comando** (Configurações → Voz): o modelo que interpreta as ordens faladas.

## Onde ver o gasto

Em Configurações → Custos:

- **Gasto desta sessão**: o total da conversa aberta agora, com o número de turnos e a repartição
  entre texto e áudio, vindos do que o serviço cobrou turno a turno. O botão **Abrir o extrato**
  mostra no Finder o arquivo do dia, guardado em Application Support/codeCanvas/voz.
- **Hoje** e **Total**, com o número de chamadas ao lado.
- **Últimos 14 dias**: o gráfico por dia.
- **Por modelo**: chamadas, tokens e custo de cada um. A linha marcada com o sinal de aproximado é
  estimativa: a API de voz não informa consumo, e o valor é calculado pelos caracteres falados.
- **Limpar extrato**: apaga os números daqui. A cobrança já feita continua na OpenAI.

Valores abaixo de um centavo aparecem com quatro casas decimais, em vez de virarem zero.
