---
slug: painel-navegador
titulo: O painel do navegador
resumo: Os controles da barra, o que a barra de endereço aceita, e o que separa o navegador que é seu do que é de um agente.
area: paineis
nivel: basico
---

Uma página web num painel do canvas, com barra de navegação própria.

## Abrir

- **`⌘K`, digitando "browser"**: abre um painel novo. Cada chamada abre mais um.
- **Por voz**: *"abre o localhost 3000"*.
- **Por um agente**, quando ele quer te mostrar uma página ou conferir o próprio trabalho. Veja
  [o agente vê o navegador](o-agente-ve-o-navegador).

O endereço em que um navegador em branco abre é escolha de cada projeto, em
[página inicial do navegador](ajustes-navegador). Em branco, ele abre no Google.

## A barra de navegação

- **Voltar** e **Avançar**: o histórico desta aba. Ficam indisponíveis quando não há para onde ir.
- **Recarregar**: relê a página **ignorando o cache**. É o comportamento de um recarregamento
  forçado, e é sempre esse: não existe um recarregamento comum aqui.
- **Parar**: substitui o recarregar enquanto a página carrega.
- **Barra de endereço**: o primeiro clique seleciona o endereço inteiro, e o clique seguinte
  posiciona o cursor.

## O que a barra de endereço aceita

- **Sem esquema**, `localhost`, `127.0.0.1`, `0.0.0.0` e `192.168.x.x` recebem `http://`. Todo o
  resto recebe `https://`.
- **Com esquema**, só `http`, `https`, `file`, `about` e `data` são carregados aqui. Um endereço com
  outro esquema é entregue ao macOS, que procura um aplicativo capaz de abri-lo.
- **`localhost:3000` é tratado como endereço**, e não como um esquema chamado `localhost`. O mesmo
  vale para `meusite.com:8080`.

## O que a página faz

- **A página sobrevive à troca de canvas**, com a mesma rolagem, o mesmo login e o mesmo histórico.
  Ela só é descartada quando o painel é fechado.
- **O zoom do canvas é o zoom da página.**
- **Uma janela nova pedida pela página** (um `target="_blank"`, o popup de login de um serviço) vira
  outro painel de navegador no canvas. Se aquela janela se fechar sozinha depois de autenticar, o
  painel se fecha junto.
- **Os sites recebem a identificação do Safari.**
- **A página que não carrega diz o motivo**, com o endereço e um botão **Tentar de novo**.

## O seu navegador e o do agente

Os cookies são separados por dono: os painéis que **você** abre dividem uma sessão entre si, e os que
um **agente** abre dividem outra. Um agente não herda o seu login, para onde quer que navegue e
independentemente de quem o mandou navegar.

## O que ele não tem

Não há favoritos, extensões, gerenciador de senhas nem sincronização com o navegador do sistema.
