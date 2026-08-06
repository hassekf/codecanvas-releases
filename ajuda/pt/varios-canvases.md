---
slug: varios-canvases
titulo: Vários canvases
resumo: Cada canvas é um projeto com a sua pasta: criar, trocar sem interromper ninguém, fechar, e a tela inicial.
area: canvas
nivel: basico
---

Um canvas é um projeto: um nome e uma pasta. Todo agente criado nele nasce nessa pasta, descrita em
[escolher o projeto](escolher-o-projeto).

## Criar

O seletor de projeto fica à esquerda da barra de comando e mostra o nome do canvas aberto. Clique
nele e escolha **Novo canvas…**.

- **A pasta é obrigatória**: o botão **Criar** fica indisponível enquanto nenhuma for escolhida.
- **O nome é opcional**: em branco, o app usa o nome da pasta.
- Na criação aparecem cinco seções: Projeto, Agentes, MCP, Navegador e Aparência. Skills, Anúncios e
  Integrações só existem depois que o projeto foi criado. Veja
  [ajustes do projeto](ajustes-projeto).
- **Por voz**, *"cria um projeto novo"* abre esta mesma janela, e a pasta se escolhe nela.

## Trocar

- **O seletor de projeto**, na barra de comando.
- **Dois toques rápidos na seta ←** volta um projeto, **dois na seta →** avança um, dando a volta no
  fim da lista. O atalho não dispara com nenhum modificador pressionado, e não dispara enquanto você
  está escrevendo num agente ou num campo de texto.
- **⌘1 até ⌘9**, pela posição do projeto na tela inicial. As teclas se trocam em
  **Configurações → Atalhos**, como está em [mover e dar zoom](mover-e-dar-zoom).
- **Por voz**: *"muda pro projeto platform"*.

Trocar não interrompe nada. Os agentes do projeto que saiu de vista continuam trabalhando e os
navegadores ficam como estavam.

## Quem está esperando noutro projeto

O seletor mostra um contador quando **outro** canvas tem agentes esperando por você. O menu dele
detalha, projeto por projeto, quantos estão esperando, quantos estão trabalhando e quantos avisos
chegaram ali enquanto você estava fora. O projeto aberto não traz essa contagem de avisos, porque
ela é zerada quando você entra nele.

## Fechar um canvas

A opção fica no fim do menu do seletor e só aparece com mais de um canvas. Ela pede confirmação, e o
que ela faz é: encerrar os agentes daquele projeto e tirar o canvas da lista. A pasta do projeto e o
código não são tocados, e não há como desfazer.

Trocar de canvas não encerra ninguém. Voltar para a tela inicial também não.

## A tela inicial

O app abre nela, e não no último projeto. Cada projeto é um cartão com a paisagem e a cor do tema
dele, o caminho da pasta, quantos agentes estão trabalhando ali agora (ou o tamanho do elenco, se
nenhum estiver) e há quanto tempo você esteve nele. O último projeto aberto ganha a marca
**ONDE VOCÊ PAROU** quando há mais de um.

- **PROJETOS RECENTES**, abaixo da grade: os cinco últimos que você abriu, em ordem de uso. Aparece
  a partir de dois projetos.
- **Editar um projeto**: o **⋯** na quina do cartão, ou o clique direito nele.
- **Voltar à tela inicial** de dentro de um canvas: **Tela inicial**, no topo do menu do seletor de
  projeto.

### A ordem dos cartões

Arraste um cartão sobre o outro para reordenar, com a moldura acesa dizendo onde ele vai cair. A
ordem fica gravada, e é ela que dá a tecla: a posição 1 responde a ⌘1, e assim por diante até a
nona. O número aparece na quina do cartão e ao lado da linha em PROJETOS RECENTES. Do décimo projeto
em diante não há tecla.

De dentro de outro canvas a tecla troca de projeto e o aviso diz o nome do que abriu. É a mesma
ordem que os dois toques nas setas percorrem.

## O que é de cada canvas

O tema, a fonte da interface, o fundo, a página em que um navegador novo abre, a conta em que os
agentes nascem, as skills, os servidores de MCP, os anúncios, as integrações e as áreas de trabalho
são de cada projeto. O Jira conectado num não aparece no outro.

O que vale para todos os projetos fica em **⌘,**, as configurações do app. Veja
[ajustes do projeto](ajustes-projeto) e [a cara do projeto](aparencia).
