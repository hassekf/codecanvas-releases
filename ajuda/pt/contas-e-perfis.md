---
slug: contas-e-perfis
titulo: Contas e perfis
resumo: Onde se cadastram as instalações do programa de agente, em qual delas cada projeto e cada agente nascem, e o que acontece com a conversa ao trocar.
area: agentes
nivel: basico
---

Uma conta é uma pasta de configuração do programa de agente. O login, os ajustes e as conversas dos
agentes ficam dentro dela.

## A lista de contas

Em **Configurações → Agentes → Instalações do Claude**.

- **A instalação padrão**: a pasta que o seu terminal já usa. Está sempre na lista e não pode ser
  descadastrada.
- **Renomear**: troca o nome de uma conta. Esse nome aparece no cabeçalho de cada agente que nasce
  nela, e só quando há mais de uma conta cadastrada. Um nome vazio devolve o rótulo original.
- **Adicionar instalação…**: abre o seletor de pastas, com os itens ocultos à mostra, e cadastra a
  pasta escolhida. Nada é copiado: o app passa a apontar para ela. O nome sugerido vem da pasta que
  contém a escolhida quando o nome desta começa com ponto. A mesma pasta não entra duas vezes.
- **Tirar da lista**: descadastra a conta. Se algum agente nasce nela, o app pergunta antes e oferece
  **Levar as conversas para a padrão** ou **Tirar e deixar as conversas lá**. Nada é apagado do disco
  nos dois casos, e as conversas voltam se você recadastrar a pasta.

Cada linha mostra o caminho da pasta e o estado dela: uma pasta nunca usada avisa que o primeiro
agente vai pedir o login, e uma pasta que saiu do disco é sinalizada como sumida.

O programa de agente de uma conta é deduzido do conteúdo da pasta, e não escolhido por você. Uma
conta pertence a um programa só. Veja [vários provedores](varios-provedores).

## A conta do projeto

Em **Editar o projeto → Agentes → Instalação do Claude**. Com uma conta só cadastrada, o menu traz a
padrão e a instrução de cadastrar as outras em Configurações.

- **A escolha vale para o canvas inteiro**: todo agente que nascer ali usa essa conta, exceto os que
  tiverem escolhido a própria.
- **Ao salvar uma troca com agentes abertos**, o app pergunta entre **Levar as conversas** e
  **Começar do zero na conta nova**, e os agentes que herdam a conta do projeto renascem nela. A
  conversa volta inteira; o turno que estava em curso naquele instante se perde. Quem escolheu a
  própria conta não é tocado.
- **Se a pasta escolhida não existir mais**, a tela avisa ali mesmo: o agente vai nascer deslogado.

## A conta de um agente

No menu do painel do agente, em **Conta do ‹nome›**. O item só aparece quando há outra conta
cadastrada do mesmo programa de agente.

- **As opções** são a conta do projeto, a instalação padrão e cada conta cadastrada. A atual vem
  marcada e não pode ser escolhida de novo.
- **Escolher não troca nada na hora**: abre uma pergunta. Se o agente já conversou, ela oferece
  **Levar a conversa** ou **Começar do zero lá**; se ele nunca conversou, só **Trocar**.
- **Levar a conversa** copia o passado dele para dentro da pasta da conta nova, e ele volta lembrando
  de tudo. Começar do zero mantém as duas contas separadas no disco. A conversa antiga não é apagada
  em nenhum dos dois casos.
- **A escolha é daquele agente**: trocar a conta do projeto depois não o arrasta junto.
- **O agente renasce na conta nova**, com o mesmo nome e o mesmo lugar no canvas. O que ele estava
  fazendo naquele instante se perde.

## Quando um agente volta sem a conversa

A conversa mora dentro da pasta da conta. Chamar um agente de volta numa conta diferente daquela em
que ele trabalhou o traz com o nome certo e a memória em branco.

O app avisa nesse caso e diz em qual conta procurou. Se a conversa estiver noutra conta cadastrada do
mesmo programa, ele diz em qual, e não a traz: trazê-la é a troca de conta descrita acima.

## Configurado em outra tela

- Os programas de agente disponíveis: [vários provedores](varios-provedores).
- Como os agentes deste canvas nascem: [ajustes do projeto](ajustes-projeto).
- Chamar de volta um agente guardado: [criar e fechar](criar-e-fechar).
