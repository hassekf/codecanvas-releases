---
slug: organizar-sozinho
titulo: Arrumar o canvas
resumo: O comando que desempilha os painéis, o modo em que o app arruma sozinho, e os arranjos guardados com nome.
area: canvas
nivel: basico
---

## Organizar agora

Quatro caminhos fazem a mesma coisa: **⌥O**, o botão de grade na barra de baixo, o `⌘K` (digite
"organizar") e a voz. A tecla se troca em **Configurações → Atalhos**, em "Organizar".

O comando arruma os painéis da área de trabalho em que você está, sem sobreposição, e **não troca o
canvas de modo**.

- **A câmera volta a 100%** e enquadra o que foi arrumado, e não o canvas inteiro.
- **Os painéis soltos ficam onde estão.** A grade se aperta para desviar deles. Um painel de design
  nunca é coberto.
- **As imagens não entram na grade.** Elas só saem de baixo dos painéis, para a vaga livre mais
  próxima, com o tamanho que tinham.
- **O aviso que aparece traz o Desfazer**, e o mesmo botão refaz o que você desfez. Ele não sobrevive
  a fechar o app.

## Deixar o app arrumando sozinho

O interruptor de dois ícones na barra de baixo alterna entre **grade automática** e **canvas livre**.
Trocar de modo também posta um aviso com Desfazer: voltar à grade descarta as posições que você
montou à mão.

Na **grade automática**:

- Os painéis preenchem a janela e se redistribuem sozinhos quando um nasce, quando um fecha e quando
  a janela muda de tamanho.
- **Arrastar um painel pelo cabeçalho o troca de lugar** com o painel cujo espaço estiver mais
  próximo de onde você soltou, dentro da mesma área. Painel solto não entra nessa troca.
- **O minimapa no canto inferior direito** abre a lista de arranjos possíveis para a quantidade de
  painéis abertos: **Automático**, uma opção para cada número de colunas (de uma até o total de
  painéis) e **Foco**, que dá o espaço maior a um painel e empilha o resto. O Foco usa o painel
  selecionado, ou o primeiro.

No **canvas livre** nada se move sozinho. Veja [os painéis e a mesa](os-paineis-e-a-mesa) e
[mover e dar zoom](mover-e-dar-zoom).

O modo, o arranjo escolhido, o painel em foco e a posição da câmera são lembrados **por área de
trabalho**.

## Arranjos guardados

### Guardar

Uma pílula com **Salvar receita** aparece sozinha quando o arranjo assenta, com um nome já sugerido.
Ela só se oferece com dois painéis ou mais na área, espera cerca de um segundo sem você mexer em
nada, some depois de alguns segundos, e não aparece se o arranjo de agora já for igual a uma receita
que você tem.

O marcador na barra de baixo abre o livro a qualquer momento, e lá há o **Guardar o de agora**.

### Voltar

No livro, **Voltar** restaura a receita da linha. Digitar o nome dela no `⌘K` e dar Enter faz o
mesmo. Cada linha diz quantos painéis a receita conhecia, quantos deles não existem mais, quantos
painéis novos vão continuar na tela, e de quando ela é.

**Restaurar nunca abre nem fecha painel: só posiciona.**

- Um painel da receita que já não existe é ignorado.
- Um painel que nasceu depois continua aberto, e é acomodado no espaço que sobrou.
- Cada painel é reencontrado pelo que ele é, e não por um número interno: um agente pela conversa
  dele, um navegador pelo endereço, um arquivo pelo caminho, uma nota por qual nota é.

No menu de cada linha há **Sobrescrever com o arranjo de agora**, **Renomear** e **Apagar**.

As receitas são de cada projeto, e guardam o arranjo da área de trabalho em que você estava.

## Pela voz

- *"organiza as janelas"*, *"tira a sobreposição"*: o mesmo que o ⌥O.
- *"põe em duas colunas"*, *"três colunas"*, *"foco no Perseu"*: troca o arranjo da grade.
- *"salva esse arranjo como revisão de PR"*: guarda uma receita com esse nome. Não mexe em painel
  nenhum.
- *"volta pro arranjo de pareamento"*: restaura a receita, sem abrir nem fechar painel.
