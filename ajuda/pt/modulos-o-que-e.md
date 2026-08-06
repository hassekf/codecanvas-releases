---
slug: modulos-o-que-e
titulo: O que é um módulo
resumo: Um painel escrito por você, que vive no canvas como os nativos e conversa com o app.
area: modulos
nivel: avancado
---

Um módulo é **um painel seu**. Você (ou um agente seu) escreve uma página, e ela passa a viver no
canvas como qualquer painel nativo: abre pelo `⌘K`, entra no arranjo, minimiza para a estante e pode
ser aberta por voz.

Serve para o que só faz sentido para você: o saldo de uma conta, o painel de uma máquina que você
administra, um contador do seu jeito, a tela de um sistema interno que ninguém mais usa.

## Onde ele mora

Numa pasta dentro da pasta do app, uma por módulo. Duas peças são obrigatórias: o manifesto, que
declara o que o módulo é, e a página inicial.

**Não há instalador nem registro.** O app vigia a pasta: criar faz o módulo aparecer, corrigir o traz
de volta, apagar o tira do app. Enquanto você escreve, salvar um arquivo recarrega os painéis daquele
módulo sem reiniciar nada.

**O módulo é da sua máquina, não do projeto.** Ele fica disponível em todos os canvases, e cada
abertura cria um painel daquele canvas: a página sabe em que projeto está, e o mesmo módulo pode
mostrar coisas diferentes em cada um.

## O que ele ganha por estar dentro do canvas

Uma página comum num navegador não consegue nada disto:

- **Fazer requisição sem restrição de origem**, porque quem busca é o app.
- **Rodar um script da própria pasta**, com a saída de volta para a página.
- **Saber em que projeto está**, e adotar o tema e a fonte daquele canvas.
- **Guardar dados** entre aberturas e entre canvases.
- **Notificar você** dentro do app, com som, leitura em voz alta e um botão que leva até o painel.
- **Dar ferramentas à Nina e aos agentes**, para que eles usem o módulo falando.

O detalhe de cada uma está em [as capacidades de um módulo](modulos-capacidades).

## O que ele não é

- **Não é uma extensão do app.** Ele desenha dentro do painel dele e não altera o resto da interface.
- **Não é distribuível.** Não há loja, registro nem instalação por link: a pasta é sua.
- **Não roda sem você.** Um módulo que precisa de segredo guarda o segredo num script da pasta, e não
  no HTML.

## Por onde seguir

- Criar um: [criar um módulo](modulos).
- O painel na tela e a lista de módulos: [o painel de um módulo](painel-modulos).
