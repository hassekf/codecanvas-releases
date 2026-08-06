---
slug: painel-gravacao
titulo: Gravar a tela
resumo: Gravar a janela do CanvasCode com áudio do app e microfone: formato, qualidade, e o que fazer com o arquivo depois.
area: paineis
nivel: basico
---

Abre pelo `⌘K` (digite "gravação" ou "gravar").

## O que entra na gravação

A **janela do CanvasCode**, o áudio que o app produz e o seu microfone. Nada que esteja por cima da
janela aparece no vídeo, e nenhum som de outro app entra. A resolução de saída vem do tamanho real
da janela em pixels, já contando o Retina.

O macOS pede a permissão de **Gravação de Tela** na primeira vez, e a gravação não começa sem ela: o
painel mostra o aviso com o caminho para autorizar. Veja
[as permissões que o macOS pede](permissoes-do-mac).

## Os controles

- **O botão central**: começa a gravar, e retoma uma gravação pausada. Enquanto grava, ele fica
  desativado.
- **Pausar**: interrompe sem encerrar.
- **Parar**: encerra e salva o arquivo.
- **O relógio** conta o tempo gravado, e a linha abaixo dele diz o estado: **Pronto para gravar**,
  **Gravando** ou **Pausado**.

Não há limite de tempo.

**A pausa não corta o trecho fora.** O tempo pausado vira um quadro parado com a duração da pausa,
no vídeo final.

## Formato da janela

Quatro botões que redimensionam a **janela do app** antes de gravar: **Paisagem · 4K** (3840×2160),
**Paisagem · 1080p** (1920×1080), **Vertical · Story** (1080×1920) e **Quadrado** (1080×1080).

## Qualidade

Os controles desta seção só funcionam com a gravação parada, e o painel diz isso quando ela está em
curso.

- **Máxima · editar**: sem alvo de taxa de bits. O arquivo é grande, e serve para quem vai editar e
  recomprimir depois.
- **Equilibrada**: o padrão. A taxa de bits acompanha o tamanho da janela.
- **Compacta · chat**: taxa menor, e a captura sai em 1×, sem Retina.
- **30 fps** e **60 fps**: quadros por segundo. 60 fps produz arquivo maior.
- **H.264 · compatível** e **HEVC · compacto**: o codec. O HEVC gera arquivo menor com o mesmo
  resultado visual; o H.264 é o que toca em mais lugares.
- **Áudio numa faixa · compartilhar** e **Faixas separadas · editar**: numa faixa, o som do app e o
  do microfone são misturados ao parar a gravação, que é o que toca em qualquer player. Separadas,
  cada fonte fica na própria faixa e o volume delas se ajusta na edição; quem abrir o arquivo sem
  editar pode ouvir só uma.

## As gravações

Os arquivos ficam em `~/Movies/codeCanvas`, em `.mp4`, com o nome pela data e hora. **Abrir a
pasta** revela essa pasta no Finder. A lista relê o disco ao abrir o painel e ao terminar uma
gravação ou uma compressão.

Cada linha traz o nome do arquivo, a data e o tamanho, e os botões:

- **Assistir aqui no canvas**: abre a gravação num painel de vídeo.
- **Abrir no player externo**: abre no player padrão do Mac.
- **Comprimir o arquivo**: abre as opções de compressão. Some enquanto outra compressão está em
  curso.
- **Mostrar no Finder**.
- **Apagar**.

**Dois cliques no nome** entram no modo de renomear. A extensão fica; nome vazio ou repetido é
recusado, e o campo continua aberto.

### Comprimir

Uma gravação por vez, com o progresso na própria linha, e os botões daquela linha somem enquanto ela
está em curso.

- **Quanto apertar**: **Equilibrada** (um arquivo gravado em Máxima encolhe em torno de 5×) ou
  **Compacta** (metade dos bits da Equilibrada; texto pequeno perde definição).
- **Onde salvar**: **Salvar como cópia**, que é o padrão e mantém o original com a versão menor ao
  lado, com "-comprimido" no nome; ou **Sobrescrever o original**, que só troca o arquivo com a
  compressão completa.

## Gravar sem abrir o painel

Em **Configurações → Interface**, a opção **Barra de gravação no rodapé** põe gravar, pausar, parar
e o tempo no rodapé do app. Ela nasce desligada, e desligá-la não afeta o painel nem os comandos de
voz.

Por voz: iniciar, pausar, retomar e parar a gravação, e pôr a janela num dos quatro formatos.

Um agente consegue listar as gravações existentes, com data, tamanho e caminho de cada uma. Veja
[o agente mexe no canvas](o-agente-mexe-no-canvas).
