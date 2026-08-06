---
slug: criar-e-fechar
titulo: Criar e fechar agentes
resumo: Abrir um agente, dispensá-lo, chamá-lo de volta com a conversa, esquecê-lo de vez, e o que acontece quando ele dorme ou cai.
area: agentes
nivel: basico
---

## Criar

- **O botão de agente novo, na barra de comando**: abre o diálogo **Novo agente**.
- **`⌘N`**: cria um Claude Code direto, com o cursor já dentro dele, mesmo enquanto você escreve para
  outro agente. **`⇧⌘N`** cria um Codex, e só funciona com o Codex ligado em
  **Configurações → Provedores**. As duas teclas se trocam em **Configurações → Atalhos**.
- **O `⌘K`**: os itens **Novo agente** e **Novo agente · Codex**, **· Grok**, **· opencode** criam
  direto, sem diálogo. Só aparecem os CLIs ligados.
- **Por voz**: *"abre um agente"*, *"sobe três agentes"*. Citar o nome de um agente que já existe
  nunca cria outro, mesmo que ele esteja guardado.
- **Um agente**, quando traz colegas para o canvas. Ver
  [um agente chama outro](um-agente-chama-outro).

## O diálogo Novo agente

- **Ferramenta**: em qual CLI o agente nasce. Só aparece com mais de um ligado.
- **Conta**: em qual instalação ele nasce. Só aparece se houver contas cadastradas para aquele CLI, e
  volta para **A do projeto** quando você troca de ferramenta. Ver
  [contas e perfis](contas-e-perfis).
- **Nome**: já vem com uma sugestão. Clicar no campo apaga a sugestão, e confirmar com o campo vazio
  usa ela mesma.
- A pasta aparece embaixo, e não se edita aqui: ela é a do canvas.

## Dispensar

Fechar o painel de um agente, pelo botão de fechar do cabeçalho ou pela tecla Delete com o canvas em
foco, encerra o processo e tira o painel da tela. Ficam guardados no projeto o nome, o CLI, a conta,
a última tarefa, o assunto que ele anotou, as entregas e a chave da conversa.

## Chamar de volta

- **No painel de elenco**, pelo botão **Chamar**. Veja [o painel do elenco](painel-elenco).
- **No `⌘K`**, digitando o nome dele.
- **Por voz**: *"chama o Hermes de volta"*. Mandar uma tarefa a um agente guardado também o traz.

Ele volta no mesmo CLI e na mesma conta em que nasceu, e a conversa continua de onde parou.

### Quando a conversa não é encontrada

- Um agente que **nunca recebeu um prompt** não tem conversa gravada, e o app não avisa nada: ele
  volta novo.
- Um agente que **já conversou** e cuja conversa não é encontrada gera um aviso dizendo em qual conta
  o app procurou.
- Se a conversa estiver em **outra conta cadastrada**, o aviso diz qual, e trocar a conta daquele
  agente é o que a traz. O app não copia nada entre contas por conta própria.

## Esquecer

Esquecer é o oposto de dispensar: o agente sai do elenco, deixa de ser chamável e o nome dele volta a
ficar livre. A pasta da conversa continua no disco.

**Só se esquece pelo [painel do elenco](painel-elenco)**, e não pelo painel do agente. Lá:

- **O botão de esquecer**, em cada linha guardada.
- **Esquecer todos**, no cabeçalho da seção **Guardados**: pede duas confirmações, porque esses têm
  conversa.
- **Liberar nomes**, no cabeçalho de **Guardados sem histórico**: esquece de uma vez os que nunca
  receberam um prompt.

## Agentes que dormem

Em **Configurações → Agentes**, **Hibernar agentes inativos** vem desligado. Ligado, o agente sem
atividade pelo tempo definido em **Dormir depois de** é encerrado, o painel fica no lugar com um botão
**Acordar**, e a conversa é retomada de onde parou quando ele volta. O conteúdo escrito no terminal
até ali se perde.

- **Dormir depois de** vai de 5 minutos a 8 horas, e vem em 1 hora. O relógio zera a cada ferramenta
  que o agente usa, a cada prompt que você manda e sempre que você abre o painel dele.
- **Nunca dormem**: quem está trabalhando, quem está esperando uma resposta sua, e o painel
  selecionado no canvas que você está vendo.
- **Mandar um prompt acorda o agente** e entrega a mensagem, sem passar pelo botão.

## Quando a API derruba um agente

O agente cortado no meio da resposta entra em estado de queda, e não em pronto. Você é avisado
conforme os seus [avisos e sons](avisos-e-sons).

Com **Retomar agentes que a API derrubar** ligado, que é o padrão, o app manda o agente continuar de
onde parou, explicando o que houve. As tentativas seguintes esperam 3 segundos, 30 segundos, 1
minuto, 2 minutos e 5 minutos, e param de crescer aí. Depois de quatro quedas seguidas o app deixa de
insistir e passa a esperar o provedor voltar. Retomar sozinho não suprime o aviso. O interruptor está
em [ajustes dos agentes](ajustes-agentes), e mandar continuar na mão está em
[falar com eles](falar-com-eles).
