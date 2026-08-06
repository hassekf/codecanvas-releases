---
slug: modulos-capacidades
titulo: As capacidades de um módulo
resumo: A ponte que o app injeta na página do módulo: rede, scripts, contexto, tema, armazenamento e notificações.
area: modulos
nivel: avancado
---

O app injeta um objeto `painel` antes de qualquer script da página. Tudo devolve uma promessa, e erro
nativo vira rejeição.

- **`painel.fetch(url, opts)`**: requisição HTTP feita pelo app, sem restrição de origem. Devolve
  status, corpo e cabeçalhos.
- **`painel.executar(script, args)`**: roda um executável da própria pasta, com ela como diretório de
  trabalho; caminho para fora dela é recusado. Devolve o código de saída, a saída padrão e a de erro,
  limitadas a 512 KB, com tempo máximo de 120 segundos. O processo recebe o workspace, o canvas e o
  módulo no ambiente.
- **`painel.contexto()`**: o módulo, o canvas e a pasta do projeto onde este painel está.
- **`painel.tema()`**: as cores de acento e a fonte do tema do canvas, para o painel não destoar.
- **`painel.guardar(chave, valor)`** e **`painel.ler(chave)`**: um armazenamento pequeno, por módulo,
  compartilhado entre os canvases. Quem quiser separar por projeto inclui o workspace na chave.
- **`painel.notificar(opcoes)`**: um aviso dentro do app, com título e corpo. As opções decidem se
  ele é fixo ou tem duração, se toca som, se é lido em voz alta, e se traz um botão que leva você até
  o painel ou traz o painel até você. Repetir o mesmo `id` reescreve o aviso no lugar em vez de
  empilhar outro; **`painel.dispensarNotificacao(id)`** o tira da tela. Ele nunca vai para a Central
  de Notificações do macOS.

Guarde tokens e senhas num script da pasta, não no HTML.

## O que a página não faz

- **Não navega**: o painel mostra o `index.html`, e um link para fora é ignorado. Imagens, CSS e
  scripts remotos carregam normalmente.
- **Não herda os seus cookies**, nem os do painel de navegador nem os do painel de mídia.

## O console é capturado

O que a página escreve no console, os erros de JavaScript e as promessas rejeitadas chegam ao app, e
um agente lê tudo isso junto com uma foto do painel. É esse o ciclo de quem está escrevendo um
módulo: editar, olhar a foto, ler o erro, corrigir.

Não existe instalar módulo de terceiro: todo módulo é escrito na sua máquina, por você ou pelos seus
agentes.
