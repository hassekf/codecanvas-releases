---
slug: minimizar-e-a-estante
titulo: Minimizar e a estante
resumo: Guardar um painel sem fechá-lo, e a lista de tudo o que está aberto neste projeto.
area: canvas
nivel: basico
---

## Minimizar

O botão **−** no cabeçalho de qualquer painel, ou o menu do botão direito → **Minimizar**.

O painel sai da tela e o conteúdo continua vivo: o agente segue trabalhando e continua mudando de
estado, e a página do navegador continua carregada, com o histórico e o que você tinha preenchido.
O aviso que aparece traz **Trazer de volta**, que o restaura e leva a câmera até ele.

Duas exceções:

- **A mídia** vira uma pílula ao lado da barra de comando, com as barrinhas de som, o play e a
  pausa. O som não para. Veja [o painel de mídia](painel-midia).
- **Um agente que trabalha num passo de uma Iniciativa** não tem o botão de minimizar. No lugar dele
  há o de ocultar, que devolve o painel para fora da sua vista sem encerrar nada. Veja
  [o painel de Iniciativas](painel-iniciativas).

## Abrir a estante

- **⌘⇧E**, que também fecha.
- **O botão da estante**, na barra de comando. Ele se destaca quando um agente guardado está
  esperando você, trabalhando ou caído.
- **O contador de painéis**, na mesma barra. Ele mostra quantos painéis estão abertos na grade
  automática, e o zoom da câmera no canvas livre.

Os dois podem ser escondidos em **Configurações → Interface**, no bloco **Itens da barra de
comando**. Escondido, o item vai para trás da seta no fim da barra.

## O que a lista mostra

O número no alto é o total de painéis deste canvas, somando todas as áreas.

- **O seletor de área**, logo abaixo do título: escolhe de qual [área de trabalho](areas-de-trabalho)
  é a lista. Ele é a mesma navegação das abas do canvas: escolher aqui troca de aba, e trocar de aba
  troca aqui. Com uma área só, ele vira um rótulo.
- **O filtro por tipo**: **Tudo**, **Agentes**, **Navegadores**, **Documentos**, **Designs** e
  **Outros**. Ele corta a lista dentro da área escolhida, e só aparece quando aquela área tem mais
  de um tipo.
- **Cada linha** traz o ícone, o nome e, quando um agente abriu aquele painel, de quem ele é. Um
  agente que não está ocioso ganha um ponto de estado ao lado do nome.
- Os painéis guardados descem para o fim da lista e continuam na área deles.

## Ir até ele, ou trazê-lo até você

- **Clicar na linha**: leva a câmera até o painel, que fica onde está. Se ele estava guardado, é
  restaurado no lugar dele e a câmera vai junto.
- **O botão de trazer**, à direita: traz o painel para o centro da sua tela e, se ele estava noutra
  área, para a área aberta. Ele só aparece onde a posição é do painel: no canvas livre, ou num
  painel solto da grade. Na grade automática o arranjo reescreveria a posição no instante seguinte.
- **O botão ao lado**: minimiza o painel, ou o tira da estante e o devolve ao lugar dele.

## Guardar e mostrar em lote

Os dois botões do rodapé agem sobre **o que está listado acima**: a área escolhida no seletor,
cortada pelo filtro.

- **Mostrar**: tira da estante todos os guardados daquela lista, cada um no lugar dele. A câmera não
  se move.
- **Minimizar**: guarda todos os que estão na tela. Só aparece a partir de dois. O aviso traz
  **Desfazer**, que devolve exatamente aqueles, e não todos os que estavam guardados.
