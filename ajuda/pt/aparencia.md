---
slug: aparencia
titulo: A aparência do projeto
resumo: Tema, paisagem de fundo, véu, papel de parede e fonte da interface, escolhidos por projeto.
area: canvas
nivel: basico
---

Tudo nesta página se escolhe na aba **Aparência** da folha de editar o projeto: abra o seletor de
projeto na barra de baixo e clique em **Editar "nome do projeto"…**. Na tela inicial, o mesmo lugar
se alcança pelo "⋯" do cartão do projeto ou pelo clique direito nele. O passeio pelos controles está
em [aparência do projeto](ajustes-aparencia).

A escolha é de cada projeto. Trocar aqui não mexe em nenhum outro.

## Os temas

São dez, num cartão cada: Meia-noite (o padrão), Grafite, Forja, Bosque, Ameixa, Enseada, Rubi,
Aurora, Terracota e Marfim. A prévia do cartão mostra o fundo daquele tema, um painel de vidro por
cima e os três sinais de estado dos agentes.

Clicar no cartão aplica o tema na tela na hora. Nada é gravado até você salvar a folha, e fechar sem
salvar devolve o que estava.

O **Marfim** é o único claro: ele vira a interface inteira para o lado claro. Duas consequências:

- **O retângulo onde o agente escreve continua escuro.**
- **A tela inicial continua escura**, por ser anterior a qualquer projeto.

## A paisagem do tema

Cada tema traz uma paisagem própria, que vem dentro do app e não é baixada. Os três botões do cartão
escolhem o que fazer com ela:

- **Animado**: o vídeo da paisagem, em loop e mudo. É o padrão. Fica indisponível no tema que não
  tiver vídeo.
- **Parado**: a paisagem congelada. Quando o tema oferece mais de uma cena, as miniaturas aparecem
  dentro do cartão dele para você escolher qual.
- **Só cor**: nenhuma paisagem, só o gradiente do tema.

Clicar num desses botões no cartão de outro tema troca o tema e o estilo de uma vez. O estilo
escolhido vale para todos os temas; a cena escolhida vale só para o tema em vigor.

O vídeo pausa sozinho quando a janela fica escondida atrás de outro app ou é minimizada.

## O véu

O controle **Escuridão do véu** decide o quanto o fundo é atenuado para o texto dos painéis
sobreviver por cima dele. Vale para a paisagem do tema e para o seu papel de parede, e vai de 0% a
100%; em 0% o fundo aparece como é.

- Ele **some da tela** quando não há fundo nenhum, ou seja, no estilo "Só cor" sem papel de parede.
- O botão **Padrão** aparece ao lado do número quando o valor está fora do padrão do tema em vigor.
- Trocar entre um tema escuro e o Marfim **move o véu junto**, e só enquanto ele ainda estiver no
  padrão do lado de onde você saiu. Depois de você mexer nele uma vez, nenhuma troca de tema o move.

## O papel de parede

No bloco **Customizar papel de parede** você põe um arquivo seu no lugar da paisagem. Ele nasce
recolhido, a não ser que já exista um papel de parede neste projeto.

- **Escolher arquivo…** aceita imagem, GIF e vídeo (MP4, MOV e M4V). Vídeo e GIF tocam em loop e
  mudos. O arquivo é **copiado para dentro da pasta do app**, então apagar o original depois não
  apaga o fundo.
- **Trocar** substitui, **Remover** devolve a paisagem do tema.
- Enquanto houver um arquivo seu, ele vence a paisagem do tema, e os botões Animado, Parado e Só cor
  deixam de mudar o que você vê. O resto do tema continua valendo.

### Pedir um fundo em vez de escolher um arquivo

O bloco **Ou peça um**, dentro do mesmo cartão, só aparece com a chave da OpenAI cadastrada em
[configurar a voz](configurar-a-voz). Você descreve o fundo e escolhe entre dois botões:

- **Buscar**: procura na web uma imagem que já existe, e devolve uma grade de candidatos para você
  clicar. É rápido, e é o caminho para algo específico e real.
- **Criar**: pinta uma imagem a partir da descrição. Leva cerca de 40 segundos, custa alguns centavos
  de dólar, e vem uma de cada vez.

## A fonte da interface

O menu **Fonte da interface** mostra cada opção escrita na própria fonte, com uma amostra abaixo. Ela
vale para o app inteiro enquanto este projeto estiver aberto.

A fonte dos **terminais** é outra, é do app inteiro, e fica em **Configurações → Terminal**, junto do
tamanho.

## O vidro dos painéis

Dois controles em **Configurações → Interface** decidem o quanto o canvas aparece atrás do texto dos
painéis. Valem para o app inteiro, e não para um projeto.

- **Desfoque do vidro dos painéis**: o quanto o fundo atrás do painel some. O controle anda em
  degraus.
- **Opacidade dos painéis**: a camada por cima do vidro, de 0% a 100%. Subir a opacidade esconde o
  efeito do desfoque.

## Pela voz

Com a assistente configurada:

- *"troca o tema pra forja"*: ela conhece os dez pelo nome.
- *"põe um fundo de floresta com neblina"*: ela **pinta** por padrão. Dizer "procura", "acha na
  internet" ou pedir algo específico e real faz ela buscar na web.
- *"procura outro"*: troca pelo próximo candidato sem você repetir a descrição. É instantâneo
  enquanto houver candidatos guardados.
- *"tira o fundo"*: remove o papel de parede e devolve a paisagem do tema.

As três primeiras precisam da chave da OpenAI.

Pedir uma **imagem** é outra coisa: ela é colada no canvas e guardada na galeria. Veja
[o painel da galeria](painel-galeria).
