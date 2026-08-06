---
slug: painel-jira
titulo: O painel do Jira
resumo: O quadro do projeto conectado dentro do canvas: filtros, arrastar cartão, detalhe do issue e o caminho até um agente.
area: paineis
nivel: basico
---

Abra com `⌘K` e **jira**, **board**, **quadro**, **issues**, **sprint**, **atlassian**, **tickets**
ou **chamados**. O painel só mostra o quadro num canvas conectado; a conexão se faz em
[Jira e Confluence](jira-e-confluence).

As colunas são as do quadro configurado no Jira, na mesma ordem. Um projeto sem quadro de software
cai nas categorias de situação do Jira.

## A barra do painel

- **O nome no alto**: o nome do site Atlassian da conexão, não o do canvas.
- **A chave do projeto**, ao lado do nome: abre a lista dos projetos que a credencial deste canvas
  alcança e troca o projeto do painel. Indisponível quando a credencial alcança um projeto só.
- **Atualizar**: recarrega o quadro.
- **Novo issue**: abre a criação de um issue. Indisponível enquanto nenhum projeto estiver escolhido.

## Filtros e busca

- **Todos**, **Meus**, **Bugs**: filtram os cartões. **Meus** compara com o nome da conta conectada;
  **Bugs** compara com o tipo do issue.
- **Responsável**: filtra por uma pessoa, entre as que aparecem no quadro. Escolher alguém estando
  em **Meus** devolve o filtro para **Todos**, e escolher **Meus** limpa o responsável: os dois se
  anulariam.
- **Mostrar etiquetas** e **Ocultar etiquetas**: mostram as etiquetas nos cartões. A escolha vale
  para todos os canvases e sobrevive ao fechar o app.
- **Buscar**: casa com o título e com a chave do issue.

O filtro rápido e o responsável ficam guardados na conexão do canvas e voltam quando você reabre o
painel. A busca não: ela some junto com o painel.

As colunas continuam todas visíveis mesmo quando um filtro esvazia uma delas. O número ao lado do
nome da coluna conta os cartões visíveis nela.

## Mover e reordenar

- **Arrastar um cartão para outra coluna**: muda o status no Jira. Recusada a mudança, o cartão volta
  ao lugar e um aviso aparece no rodapé do painel por alguns segundos.
- **Soltar um cartão sobre outro da mesma coluna**: reordena os dois no Jira. Entre colunas
  diferentes, o mesmo gesto vale como mudança de status.

## O cartão

- **Clicar**: abre o detalhe do issue.
- **Abrir detalhes**, no menu **⋯**: o mesmo detalhe.
- **Enviar para um agente**, no menu **⋯**: só aparece com algum agente aberto no canvas.
- **Copiar a chave**, no menu **⋯**: copia a chave do issue.
- **Arrastar o cartão para dentro de um painel de agente**: digita a chave e o título na caixa dele,
  **sem** enviar, e põe o agente em foco. Você completa a frase e envia. A partir da chave o agente
  lê o issue inteiro sozinho.

## O detalhe do issue

- **Status**: vira um menu com as transições que o Jira permite ali. Sem permissão de transição, é
  só um campo de leitura.
- **O lápis**: edita o título e a descrição. Só aparece com permissão de edição. A descrição só é
  reenviada ao Jira se você mexer nela, para a formatação original não se perder ao salvar apenas o
  título.
- **Anexar**: envia um arquivo ao issue.
- **Comentar**: `Enter` envia, `Shift+Enter` quebra linha. O campo só existe com permissão de
  comentar.
- **Uma imagem anexada ou embutida num comentário**: clicar amplia; ampliada, **Enviar para o
  canvas** cola a imagem no canvas.
- **Um link na descrição ou num comentário**: pergunta entre **Abrir aqui**, que abre num painel de
  navegador deste canvas, e **No navegador externo**.
- **Enviar para um agente**, no rodapé: manda a menção e fecha o detalhe.
- **Copiar a chave** e **Abrir no Jira**, no rodapé: a chave para a área de transferência, e a página
  do issue no seu navegador.

Mudar status, comentar e editar aparecem na tela antes de o Jira confirmar. Se a chamada falhar, o
valor anterior volta e um aviso conta o que aconteceu.

## Novo issue

- **Espaço**: o site e o projeto deste canvas, já escolhidos.
- **Tipo do ticket**: os tipos que o projeto aceita, carregados do Jira ao abrir.
- **Status**: a coluna em que o issue nasce. O app cria o issue e depois tenta movê-lo para lá; sem
  transição disponível, ele fica onde nasceu.
- **Resumo**: obrigatório.
- **Descrição**: opcional.

Criado, o cartão sobe para o topo da coluna.

## Quando o painel não tem o que mostrar

- **Sem conexão**: o botão **Conectar o Jira** abre a edição deste workspace na parte da Atlassian.
- **Sem projeto escolhido**: o botão **Escolher o projeto** leva ao mesmo lugar.
- **Projeto sem issues**: o painel diz isso, e **Novo issue** continua disponível.

## Configurado em outra tela

- A conexão, o projeto e os avisos do Jira: [Jira e Confluence](jira-e-confluence).
- O atalho para a conexão, dentro das Configurações: [Integrações](ajustes-integracoes).
