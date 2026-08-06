---
slug: ajustes-projeto
titulo: Ajustes do projeto
resumo: A janela do canvas: a máquina onde ele mora, a pasta em que os agentes nascem, o nome, e as outras seções.
area: projeto
nivel: basico
---

Abra o seletor de projeto, à esquerda da barra de comando, e escolha **Editar “nome do projeto”…**.
Na tela inicial, o mesmo se alcança pelo **⋯** na quina do cartão ou pelo clique direito nele.

A janela tem um menu lateral, e a primeira seção é **Projeto**.

## Onde este projeto mora

- **Nesta máquina**: a pasta é uma pasta do seu Mac.
- **Num servidor meu**: o projeto e os agentes ficam noutra máquina, que continua trabalhando com o
  Mac desligado. Escolhido isto, o controle da pasta local desaparece. Veja
  [canvas remoto](canvas-remoto).

## Pasta do projeto

Todo agente deste canvas nasce nesta pasta, e é ela que o Git, os arquivos e o navegador dos agentes
enxergam. O botão **Escolher…** abre o seletor de pastas do macOS.

Trocar a pasta com agentes de pé:

- Um aviso aparece na própria seção, antes de você salvar, dizendo quantos agentes estão rodando na
  pasta antiga.
- Ao salvar, o app pergunta o que fazer com eles. **Reabrir com a conversa** encerra e recria cada
  agente na pasta nova levando a conversa junto: ele volta lembrando de tudo, mas o que estava
  fazendo naquele instante se perde. **Deixar na pasta antiga** mantém os processos vivos onde
  estão, e só os próximos agentes nascem na pasta nova.
- Quando algum agente não puder levar a conversa, o app diz quais são, pelo nome, e quantos voltam
  inteiros, antes de mexer em qualquer coisa. Dali dá para reabrir mesmo assim ou cancelar. A
  conversa antiga não é apagada em nenhum dos casos.

## Nome

É por ele que você chama o projeto no seletor, na tela inicial e por voz. Em branco, na criação, o
app usa o nome da pasta.

## Trocar a conta do projeto

Se a conta em que os agentes nascem mudar e houver agentes vivos que a herdam, o app pergunta o que
fazer com a conversa deles: **Levar as conversas** copia o passado de cada um para dentro da pasta
da conta nova, e **Começar do zero na conta nova** deixa esse passado onde está. Nada é apagado da
conta antiga, e quem escolheu a própria conta no menu do painel não é afetado. Veja
[contas e perfis](contas-e-perfis).

## As outras seções

- **Agentes**: a instalação do Claude em que os agentes deste projeto nascem, as flags com que
  nascem, se abrem páginas no navegador interno ou no externo, e o isolamento por worktree. Veja
  [contas e perfis](contas-e-perfis) e [worktrees e isolamento](worktrees-e-isolamento).
- **Skills**: as capacidades que os agentes daqui podem usar. Veja
  [ajustes de skills](ajustes-skills).
- **MCP**: os servidores de ferramentas que os agentes daqui sobem. Veja
  [ajustes de MCP](ajustes-mcp).
- **Navegador**: a página em que um navegador novo abre. Veja
  [ajustes do navegador](ajustes-navegador).
- **Aparência**: o tema, a fonte da interface e o fundo deste canvas, mais o contorno do painel
  selecionado, que vale para todos os canvases. Veja [aparência do projeto](ajustes-aparencia).
- **Anúncios**: os alertas que os agentes disparam na sua tela ao cumprir uma regra sua. Veja
  [anúncios](ajustes-anuncios).
- **Integrações**: as conexões deste projeto, como o Jira. Veja
  [integrações](ajustes-integracoes).

Ao **criar** um canvas, Skills, Anúncios e Integrações não aparecem no menu lateral: as três
precisam de um projeto que já existe. Elas surgem assim que você salva.

## A prévia da aparência

Enquanto esta janela está aberta, mexer no tema, no papel de parede ou na escuridão do véu muda o
canvas atrás dela na hora. Só o botão **Salvar** grava a escolha: **Cancelar**, o Esc e o clique
fora devolvem a aparência que estava lá antes.

## Isto não é o mesmo que Configurações

**⌘,** abre as configurações do app: a voz, o microfone, os atalhos, a escala da interface, a fonte
dos terminais, a largura máxima de um painel, as notificações. Tudo isso vale para todos os
projetos. O que você edita nesta janela vale só para este canvas.
