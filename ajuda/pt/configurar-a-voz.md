---
slug: configurar-a-voz
titulo: Configurar a voz
resumo: A chave da OpenAI, o microfone, quem fala com você, os timbres e as teclas da voz.
area: nina
nivel: basico
---

Em **Configurações → Voz**. A chave e os ajustes da conversa ficam em **Configurações → Conversa**.

## A chave da OpenAI

Em Configurações → Conversa.

- **Chave da OpenAI**: guarda a chave no Keychain do macOS. O valor ao lado do título mostra
  "configurada" ou "faltando", e a chave nunca é exibida de volta. Salvar dispara a busca dos modelos
  que a sua conta tem, para a conversa e para as imagens.

Sem chave, ficam indisponíveis a Nina, a voz natural e o modelo do comando. O ditado, a voz do
sistema e [a conversa escrita](a-nina-por-texto) não dependem dela.

## O microfone

- **Modelo de transcrição**: escolhe como a sua fala vira texto. "Sistema (Apple)" é o padrão e
  mostra o texto enquanto você fala. "Parakeet v3" baixa cerca de 600 MB uma vez e transcreve quando
  você solta a tecla. Veja [ditado](ditado).
- **Microfone**: escolhe o dispositivo de entrada. "Padrão do sistema" segue os Ajustes do Sistema e
  diz entre parênteses qual dispositivo é esse. Um dispositivo escolhido e depois desconectado
  aparece como "desconectado", em vez de ser trocado em silêncio.
- **Ganho do microfone**: multiplica o sinal de entrada, de 1× a 24×. O padrão é 1×.
- **Testar o microfone**: mostra o áudio que chega, já com o ganho aplicado, e marca com um traço o
  limiar a partir do qual a fala é detectada. O medidor acompanha o ganho enquanto você arrasta o
  controle, e para de gravar quando você fecha as Configurações.
- **Saída de áudio**: escolhe o dispositivo de saída. O app ainda não usa esta escolha.

## Quem fala com você

Os três interruptores deste cartão funcionam em cascata: o app fala com a voz natural; quando ela não
pode, com a voz do sistema; sem as duas, não fala.

- **A Nina**: liga a conversa por voz (⌥C), o bom-dia e a resposta falada aos agentes. Indisponível
  sem a chave.
- **Voz natural**: usa a voz da OpenAI nos avisos e nas confirmações do modo comando. Indisponível
  sem a chave.
- **Voz do sistema**: usa a voz do macOS, sem chave e sem internet. É ela que fala quando a voz
  natural não pode.

Com os três desligados, o cartão mostra "silêncio" e tudo o que seria falado vira notificação na
tela. O ditado continua funcionando: ele é transcrição, não fala.

## Os avisos falados

Em Configurações → Voz. Valem para os avisos e para a confirmação do modo comando, não para a Nina.

- **Volume da voz**: 10% a 100%, padrão 70%. Afeta só a voz do app, e não o volume do Mac.
- **Velocidade dos avisos**: 0,80× a 1,60×, padrão 1,00×. Acima de 1,4× a voz começa a comer o fim
  das palavras.
- **Timbre**: escolhe a voz da nuvem. O botão "Ouvir" toca uma amostra pelo mesmo caminho de um aviso
  real, com o volume e a velocidade escolhidos. Indisponível com a voz natural desligada.
- **Modelo da voz**: escolhe o modelo de síntese. Indisponível com a voz natural desligada.
- **Modelo do comando**: escolhe quem interpreta a frase do [modo comando](o-modo-comando). Depende
  da chave, e não da voz natural: ele trabalha mesmo com o app mudo.

## A voz da Nina

Em Configurações → Conversa. Estes valem só para a conversa por voz.

- **Modelo da Nina**: o modelo da conversa. O botão "Atualizar" refaz a lista a partir da sua conta.
- **Voz da Nina**: o timbre dela, com um botão "Ouvir" que toca a amostra sem abrir conversa. O
  padrão é Marin.
- **Velocidade da Nina**: 0,80× a 1,60×, padrão 1,00×.
- **Nome da assistente**: como você a chama, e como ela se apresenta entre os agentes. O padrão é
  Nina.
- **Silêncio para ela responder**: quanto silêncio ela espera antes de assumir que você terminou de
  falar. De 300 a 3000 ms, padrão 900 ms.
- **Sensibilidade do microfone**: de que volume para cima o som conta como voz. De 0,10 a 0,90,
  padrão 0,50.

## As teclas

Os padrões de fábrica:

- **⌥D**: [ditar](ditado) para um agente.
- **⌥X**: [mandar o canvas fazer](o-modo-comando).
- **⌥C**: abrir e fechar [a conversa por voz](falar-com-a-nina).
- **⌘J**: abrir e fechar [a conversa escrita](a-nina-por-texto).
- **Esc**: cancelar o que estiver no ar, seja o ditado, o comando, a conversa ou a voz que está
  falando. O texto de um ditado cancelado é descartado e não chega a agente nenhum.
- **⌥F**: virar os painéis e mostrar o resumo de cada agente.
- **⌥O**: organizar os painéis sem sobreposição.

Todas se trocam em **Configurações → Atalhos**: clique no campo da linha e aperte a combinação nova.
A tela avisa quando duas ações ficam na mesma tecla, dizendo quais são; nesse caso uma delas deixa de
funcionar. O Espaço é evitado nos atalhos de voz porque o Claude Code já usa "segurar espaço" para
ditar dentro do terminal.

As teclas de voz valem com o CanvasCode na frente, inclusive com o cursor dentro de um agente. Com o
app atrás de outra janela, a tecla é do app que está em uso. A exceção é o Esc, que vale no Mac
inteiro enquanto há voz no ar.

**Enquanto as Configurações estão abertas, as teclas de voz não disparam.** Elas voltam ao ar, já com
os valores novos, quando a folha fecha, por qualquer caminho.

## Quando você fala e nada acontece

- O sinal fraco demais nunca cruza o limiar de detecção: suba o **ganho do microfone** até o teste
  acusar a sua fala em volume normal.
- O ruído da sala que nunca deixa silêncio impede o turno de fechar, e a Nina não responde: suba a
  **sensibilidade do microfone**. Se ela perde o começo das suas frases, desça.
- O microfone depende da permissão do macOS. Em **Configurações → Diagnóstico** estão o estado de
  cada permissão, o botão que a pede de novo e um que apaga o registro de permissões deste app para
  o sistema perguntar do zero, com o app reaberto depois. Ver
  [as permissões do macOS](permissoes-do-mac).
