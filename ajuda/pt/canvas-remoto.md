---
slug: canvas-remoto
titulo: O canvas num servidor
resumo: Como apontar um projeto para outra máquina, o que o teste de conexão verifica, o que acontece quando a rede cai e o que ainda não funciona à distância.
area: integracoes
nivel: avancado
---

Um canvas pode viver noutra máquina. Os agentes nascem e trabalham lá, e este Mac é a vista. O app
chega ao servidor por SSH, e não instala nem deixa nada escutando do outro lado.

Esta parte do CanvasCode está em construção. O que ainda não funciona está no fim da página.

## Escolher a máquina

Em **Editar o projeto → Projeto → Onde este projeto mora**.

- **Nesta máquina** e **Num servidor meu**: decidem onde os agentes deste canvas trabalham. Escolher
  o servidor esconde o campo da pasta local.
- **O menu de servidores** lista os cadastrados e traz **Adicionar servidor…**. Um servidor
  cadastrado pertence ao app, e não ao canvas: a mesma máquina serve a vários projetos.
- **Trocar de servidor limpa a pasta escolhida.**
- **Editar…**: reabre o cadastro daquele servidor.

## Cadastrar um servidor

- **Apelido**: como esse servidor aparece na lista e como a voz o chama.
- **Endereço**: o IP ou o domínio, o usuário e a porta do SSH.
- **Chave**: o caminho da chave privada. Em branco, o app usa a chave com que você já entra nessa
  máquina.
- **Testar conexão**: diz se alcançou a máquina, qual é o sistema, e se estão lá o git, o tmux, o
  node e o programa de agente. Quando o programa de agente está instalado mas sem credencial, o teste
  avisa: sem isso o agente sobe, fica calado e parece travado.
- **Salvar** fica indisponível enquanto o endereço estiver vazio.

## Escolher a pasta

**Escolher pasta…** abre um navegador pelas pastas do servidor.

- **Acima** sobe um nível, e **Nova pasta…** cria uma pasta ali.
- **As pastas que são repositório** vêm marcadas.
- **Usar esta pasta** fecha o navegador com a escolha. O app prepara o resto sozinho.

## O que funciona igual

- **O terminal de cada agente**, com a tela inteira dele.
- **O estado do agente**: a luz do painel, o assunto, quem escreveu em cada arquivo, a pergunta
  pendente.
- **O Git do repositório de lá**, no painel de sempre.
- **A gaveta de arquivos**, e abrir um arquivo num painel para ler.
- **Arrastar um arquivo para um agente**: o arquivo sobe para o servidor primeiro, e o agente recebe
  o caminho de lá. Se o envio falhar, nada é colado no prompt e o app diz o motivo.

## Quando a rede cai

A queda da conexão não encerra o agente: a sessão continua viva no servidor.

- **O aviso aparece na tela do próprio painel**, dizendo qual conexão caiu e em quantos segundos o
  app tenta de novo.
- **A espera cresce a cada tentativa**, de 3 segundos até o teto de 30.
- **Ao religar, a sessão é reencontrada** com o histórico e a pergunta pendente onde estavam.
- **Um painel fechado não religa.** O agente continua vivo no servidor, e você o traz de volta como
  qualquer agente guardado.

## Se você entra como root

O programa de agente se recusa a rodar como root com as permissões liberadas. Nesse caso o app tira
essa opção: o agente sobe e volta a pedir permissão antes de cada ferramenta, e o app trata esses
pedidos como sempre. O teste de conexão avisa quando o usuário é root.

## O que ainda não funciona

- **Editar um arquivo remoto**: o painel abre e mostra o conteúdo, e o botão de editar não aparece.
- **Acompanhar um arquivo remoto ao vivo**: ele não é vigiado como o daqui, e se relê quando você
  pede.
- **O navegador do agente é um painel deste Mac.** Sem o Mac ligado, o agente remoto fica sem ver a
  página que produziu.
- **Os módulos são servidos pelo app**, e portanto só existem com o Mac ligado.
- **Os painéis de Uso e de Desempenho** medem esta máquina.
- **Dois Macs no mesmo canvas** ainda não se combinam.

## Configurado em outra tela

- A pasta de um projeto local: [ajustes do projeto](ajustes-projeto).
- Trocar de projeto: [escolher o projeto](escolher-o-projeto).
