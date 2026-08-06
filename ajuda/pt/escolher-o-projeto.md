---
slug: escolher-o-projeto
titulo: Escolher o projeto
resumo: Criar um projeto, apontar a pasta, trocar de projeto, e o que acontece com os agentes quando a pasta muda.
area: comecando
nivel: basico
---

Um projeto é uma pasta do seu disco. **Todo agente do projeto nasce dentro dela**, e é essa pasta que
o Git, os arquivos e o navegador dos agentes enxergam.

## Criar

Na tela inicial, **Novo projeto**. A folha tem cinco abas, e só a primeira é obrigatória:

- **Projeto**: onde o projeto mora (nesta máquina ou num servidor seu), a pasta e o nome. Sem pasta
  escolhida, o botão **Criar** fica indisponível.
- **Agentes**: em que instalação do Claude os agentes deste projeto nascem, e as flags passadas a
  eles. Veja [ajustes dos agentes](ajustes-agentes).
- **MCP**: os servidores que os agentes deste projeto sobem. Veja [ajustes de MCP](ajustes-mcp).
- **Navegador**: a página em que um navegador novo abre aqui. Veja
  [ajustes do navegador](ajustes-navegador).
- **Aparência**: o tema, a fonte da interface e o fundo. Veja [aparência](aparencia).

As abas de **Skills**, **Anúncios** e **Integrações** só existem depois que o projeto foi criado:
elas dependem de um projeto de verdade no disco.

O projeto pode morar noutra máquina, com este Mac como vista. Veja
[canvas remoto](canvas-remoto).

## Trocar de projeto

- `⌘1` a `⌘9` abrem os projetos pela posição deles. A tecla aparece na quina de cada cartão da tela
  inicial. O modificador e o mapa são trocáveis em Configurações → Atalhos.
- `⌘K` acha um projeto pelo nome. Veja [busca e comandos](busca-e-comandos).
- Na tela inicial, os projetos aparecem como cartões, com o caminho da pasta, quantos agentes estão
  trabalhando agora e quando você esteve ali pela última vez. O último aberto vem marcado.

Nada se perde na troca: os painéis continuam onde estavam e os agentes seguem rodando.

## O que é de cada projeto

- os canvases, as áreas de trabalho e os painéis abertos;
- os agentes, na tela e guardados;
- o tema, a fonte da interface e o fundo. Veja [aparência](aparencia);
- as skills e os servidores MCP ativos;
- os anúncios;
- as integrações. O Jira de um projeto não aparece em outro. Veja
  [ajustes de integrações](ajustes-integracoes).

Um mesmo projeto pode ter vários canvases. Veja [vários canvases](varios-canvases).

## Mudar a pasta depois

A pasta se troca em [ajustes do projeto](ajustes-projeto).

**A pasta de um agente é a pasta em que o processo dele nasceu**, e trocar o campo não alcança um
terminal que já está de pé. Com agentes rodando, o app avisa antes de salvar e pergunta:

- **Reabrir com a conversa**: cada agente é encerrado e recriado na pasta nova, levando a conversa
  junto. Ele volta lembrando de tudo, e o que estava fazendo naquele instante se perde.
- **Deixar na pasta antiga**: os processos continuam vivos onde estão, e só os próximos agentes
  nascem na pasta nova.

Quando a conversa de algum agente não puder ser levada, o app diz quais antes de mexer em qualquer
coisa, e você decide se continua.
