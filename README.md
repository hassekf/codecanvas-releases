# codeCanvas — releases

Este repositório existe só para **distribuir** o codeCanvas: ele guarda o `appcast.xml`
(o feed que o app consulta para se atualizar) e os instaladores de cada versão.

O código-fonte é privado e vive em outro lugar.

## Baixar

Pegue o DMG mais recente em [Releases](https://github.com/hassekf/codecanvas-releases/releases),
abra, e arraste o **codeCanvas** para a pasta Aplicativos.

O app é assinado com Developer ID e notarizado pela Apple, então ele abre normalmente — sem
diálogo de "desenvolvedor não identificado". Daí em diante ele se atualiza sozinho.

## Por que um repo separado

O feed do Sparkle precisa de uma URL **pública**: um repositório privado devolve 404 para
quem não tem token, e um auto-update que não acha o feed é um auto-update que não existe.
Separar a distribuição do código resolve isso sem abrir o código.

Cada atualização publicada aqui é assinada com uma chave EdDSA cuja metade privada nunca sai
do Mac de quem publica. O app carrega a metade pública e **recusa** qualquer binário que não
bata — sem isso, quem dominasse este repositório poderia empurrar um app qualquer para todo
mundo que tem o codeCanvas instalado.
