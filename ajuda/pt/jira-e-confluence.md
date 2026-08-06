---
slug: jira-e-confluence
titulo: Jira e Confluence
resumo: Conectar um projeto à sua conta Atlassian, escolher o projeto do Jira, ligar os avisos e desconectar.
area: integracoes
nivel: basico
---

Na edição do projeto, em **Integrações → Atlassian**. Você chega lá pelo seletor de projeto, à
esquerda da barra de comando, em **Editar "<nome>"…**, ou pelo atalho de
[Integrações](ajustes-integracoes) nas Configurações.

A conexão é de cada canvas: a conta, o site e o token ficam com aquele projeto, e nenhum outro canvas
os enxerga. O token é gravado no Keychain do seu Mac, nunca num arquivo do app.

## Conectar

- **Site**: o endereço da sua Atlassian, no formato `empresa.atlassian.net`.
- **Email**: o email da sua conta.
- **Token de API**: gerado em `id.atlassian.com`, em Segurança → Tokens de API. Ele vale por site.
- **Trazer o Confluence junto**: mesmo token, mas a base de documentação é uma escolha à parte.
- **Conectar**: valida as credenciais. O campo do token é limpo depois de conectar.

Conectado, a seção **Conectado** mostra o site e o nome da conta, e diz se o Confluence entrou.

## O projeto do Jira

- **Projeto do Jira**: o menu lista os projetos que a credencial alcança. É esse projeto que o painel
  abre e o que a Nina assume quando você não diz qual. **Nenhum** desfaz a escolha. Ao lado do
  rótulo, o app mostra quantos issues estão abertos ali.

Sem projeto escolhido, os avisos abaixo ficam indisponíveis: não há sobre o que perguntar.

## Os avisos do Jira

O Jira da nuvem não entrega as suas notificações pessoais a um aplicativo, então quem pergunta é o
app, de tempos em tempos, e só sobre o projeto deste canvas. O aviso é sempre escrito: uma
notificação no canvas e, com o app em segundo plano, uma do macOS. Nunca falado.

- **Me avisar do Jira**: o interruptor geral deste projeto. Desligado, o app não faz nenhuma chamada.
  Nasce desligado.
- **Mencionaram você**: alguém escreveu o seu nome num comentário. É o único que traz a chave e o
  título do cartão, e o único que já vem ligado.
- **Passaram um cartão para você**: você virou o responsável por um cartão que era de outra pessoa,
  ou de ninguém.
- **Criaram um cartão no projeto**: todo cartão novo, seu ou não.
- **Perguntar ao Jira a cada**: 5, 15, 30 ou 60 minutos. O padrão é 15, e menos de 5 não é oferecido.

A primeira varredura de um projeto não avisa nada: ela marca o instante e conta dali em diante.
Depois de um tempo com o app fechado, o app olha no máximo as últimas 24 horas.

## O que fica disponível depois

- **O quadro no canvas**: as colunas do Jira, arrastar para mudar de status, criar issue. É o
  [painel do Jira](painel-jira).
- **Por voz**: *"o que tem no board?"*, *"quais os bugs abertos?"*, *"move a PROJ-12 pra pronto"*.
- **Para os agentes deste canvas**: ler o quadro, abrir um issue inteiro com os comentários, criar e
  mover.
- **Buscar no Confluence**: só com o interruptor do Confluence ligado.

As quatro ferramentas de voz formam o grupo **Jira e Confluence** em Configurações → Ferramentas:
desligá-lo mantém a conexão de pé e tira o Jira das mãos da Nina. Num canvas desconectado, elas nem
chegam a ser enviadas ao modelo.

## Desconectar

- **Desconectar**: apaga o token do Keychain e a conexão daquele canvas. As ferramentas de voz somem,
  os agentes perdem o acesso e o painel do Jira fica sem o que mostrar.
