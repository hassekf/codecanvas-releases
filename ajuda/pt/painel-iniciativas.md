---
slug: painel-iniciativas
titulo: O painel de Iniciativas
resumo: As três telas do painel, o que cada botão de uma execução faz, e o que acontece quando ela para em você.
area: iniciativas
nivel: avancado
---

Abra com `⌘K` e **iniciativas**, **runs**, **execuções**, **esteira**, **workflow**, **passos** ou
**portão**.

Uma Iniciativa é um processo escrito num arquivo de `.codecanvas/iniciativas/` do repositório. Uma
**run** é uma execução dele.

## Quando não existe nenhuma

O painel mostra o que encontrou no repositório sem agente nenhum (comandos, scripts de validação,
execuções antigas) e dois botões. Nos dois você escolhe o agente, e a conversa acontece no painel
dele:

- **Escrever do zero, conversando**: o agente recebe o aviso de que vocês vão desenhar um processo.
- **Ler o projeto e propor**: o agente recebe também o que o painel encontrou, e propõe.

## A lista

- **Todas**, **Rodando**, **Esperam você**, **Esperam fora**, **Concluídas**: filtram as runs. Cada
  um traz a contagem.
- **O menu de Iniciativa**: restringe a lista a uma delas. Só aparece com mais de uma Iniciativa no
  projeto.
- **Nova iniciativa**: escolhe um agente e abre a conversa para escrever uma.
- **Nova run**, na linha de uma Iniciativa: começa uma execução.
- **Arquivar**, na linha de uma run terminada: tira a run da lista sem apagar a pasta dela.
- O botão à direita de cada run muda com a situação dela: **Responder**, **Resolver**, **Ler o que
  travou**, **Retomar**, **Ver o que falta**, **Ver o resultado**.

Uma Iniciativa que mora numa [worktree](worktrees-e-isolamento) aparece com a branch ao lado, e as
runs dela acontecem lá dentro.

Um arquivo que o app não conseguiu ler **aparece na lista mesmo assim**, marcado, e a tela dele
lista cada recusa com o campo e o motivo. O menu dela oferece **Ver os problemas**, **Pedir a um
agente que conserte** e **Abrir o arquivo**.

## A tela de uma Iniciativa

Mostra os passos na ordem, o que cada um recebe e produz, quem executa (um comando ou um agente), os
portões, as revisões, o teto de voltas de cada rota e o que a Iniciativa pede para começar.

- **Nova run**: começa uma execução.
- **Editar com um agente**: manda o arquivo e o que você quer mudar ao agente que escolher.
- **Ver as origens**: os arquivos do projeto de onde a Iniciativa saiu, cada um marcado como
  **aponta** (a run lê a versão de agora) ou **cópia** (a run usa a versão gravada na Iniciativa).
- **Ver o que mudou**: aparece quando um arquivo de origem mudou depois que a Iniciativa foi
  escrita. **Reler com o agente** manda a ele o arquivo, o que mudou e a Iniciativa que veio dali.
- **Arquivar as concluídas** e **Apagar a Iniciativa**, no menu: apagar manda o arquivo `.json` para
  o lixo; as runs no histórico e os arquivos do projeto continuam onde estão.

## Começar uma run

**Nova run** pede o que a Iniciativa declarou precisar: uma fonte (um link, uma chave de cartão, um
arquivo), um texto, uma lista de perguntas, a saída de outra run, ou nada. Sem essa entrada, o botão
de começar fica indisponível.

Na mesma tela:

- **O nome da run**: sugerido a partir do que você deu, editável. A tela diz se o nome já existe, e
  nesse caso acrescenta um sufixo.
- **Com qual ferramenta**: o provedor dos agentes dos passos que não fixam o seu.
- **Sozinha até precisar de você**: encadeia os passos e só para nos portões que pedem você, ou se
  um portão travar.
- **Passo a passo**: para depois de cada passo e espera você mandar seguir.
- **Onde o código acontece**: isola numa worktree própria os passos que escrevem código, com a
  branch e a pasta escritas na tela. As instruções dos agentes vêm deste canvas ou de
  [configurações dos agentes](ajustes-agentes), e **personalizar** as troca só para esta run.
- **Começar a run**.

## Enquanto a run anda

- **Cada passo** nasce com um agente próprio, sem painel. Clicar no passo abre o painel dele;
  minimizar o esconde de novo.
- **Ver painel do agente**: o mesmo, pelo botão.
- **Pausar após este passo** e **Deixar correr até o fim**: trocam o modo da run em andamento.
- Quem roda o portão de um passo é o app, depois que o agente diz que terminou. Reprovado, o
  trabalho volta ao agente com o motivo, até o teto de voltas daquela rota.
- Se o agente de um passo morrer, o app põe outro no lugar até duas vezes. Na terceira, a run para e
  diz que o problema foi a queda.
- Fechado o app com uma run andando, ela aparece como interrompida na volta, e **Retomar daqui**
  a religa.
- **Encerrar a run**, no menu: interrompe o que estiver acontecendo. Os artefatos já escritos, a
  worktree e os commits ficam; uma run encerrada não volta a andar.

## Quando a run para em você

- **Assinatura**: a tela mostra o que a Iniciativa mandou mostrar (o documento, a prévia do que vai
  acontecer fora do canvas, ou o pedido escrito). O botão de aprovar leva o rótulo que a Iniciativa
  escreveu. **Devolver com um comentário** abre o campo e devolve o passo com o seu texto; devolver
  sem escrever nada não é possível.
- **O agente perguntou**: a pergunta apareceu no meio do passo e não estava no processo. Responder
  não aprova nada nem avança o passo; o texto chega ao agente no próximo turno dele.
- **Espera alguém de fora**: a tela diz o que o passo está esperando. Você pode soltar o arquivo,
  colar um link ou escrever o que chegou, e **Chegou, pode seguir** libera. **Copiar o pedido** copia
  o que falta, para você mandar a quem estiver com a bola.
- **Travou**: o teto de voltas estourou, ou o comando do portão não estava onde a Iniciativa disse.
  Os botões são **Tentar o portão de novo**, **Seguir sem o portão passar**, **Dar mais 3 voltas** e
  **Mais 3, com um agente novo**. Quando o comando do portão não existe, nenhuma volta é gasta e a
  tela diz onde o app procurou.
- **Passo a passo**: no fim de cada passo a tela mostra quem faria o próximo, o que entra e o que
  sai, e espera o botão de seguir.

## Quando termina

A tela da run mostra os artefatos, onde eles ficaram (a pasta ou a branch), quantas assinaturas suas
teve e como cada portão passou. **Rodar de novo** começa outra run da mesma Iniciativa. O que a
Iniciativa declarou fazer com o resultado é oferecido como botão, nunca executado sozinho.

## Ficar sabendo com o painel fechado

- **A pastilha na barra de comando**: conta as execuções vivas do projeto e abre a lista delas, com a
  run e o passo de cada uma. Ela conta o que está vivo, e não o que está trabalhando. Por padrão fica
  sempre visível e serve de atalho; **Esconder as Iniciativas quando não há nada pendente**, em
  Configurações → Interface, faz com que só apareça durante uma execução.
- **Os avisos**: a run avisa quando termina, quando para esperando você, quando faz uma pergunta,
  quando trava e quando chega o que ela esperava de fora. Passar de um passo para o outro não avisa.
  Clicar no aviso abre aquela run. Com o painel da run à vista, o aviso não é lido em voz alta. Os
  interruptores de som, voz e notificação do macOS são os de [avisos e sons](avisos-e-sons).

## Limitações

- **Editar a Iniciativa com uma run andando muda a execução em curso.** A tela da run avisa quando
  isso aconteceu.
- **Uma Iniciativa é feita dos comandos e scripts daquele repositório**, e não é reaproveitável em
  outro projeto.
