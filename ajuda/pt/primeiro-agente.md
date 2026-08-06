---
slug: primeiro-agente
titulo: O primeiro agente
resumo: Instalar o programa de agente, criar o painel, mandar a primeira tarefa e ler o estado dele.
area: comecando
nivel: basico
---

Um agente é o programa de linha de comando rodando dentro de um painel, com o terminal inteiro
funcionando.

## Instalar o programa de agente

Se o Claude Code não estiver na máquina, o painel do agente novo mostra **Instalar agora**. A
instalação é local e não pede senha de administrador.

Enquanto o painel diz **Preparando o agente…**, o app está descobrindo onde o programa mora. Leva
alguns segundos.

Outros programas de agente rodam no mesmo canvas: Codex, Grok e opencode. Cada um é ligado em
Configurações → Provedores. Veja [vários provedores](varios-provedores).

## Criar

- `⌘N`. Funciona mesmo com o cursor dentro de outro agente, e o painel novo já nasce com o cursor
  dentro dele.
- `⌘⇧N` cria um agente do Codex, e a tecla só faz algo com o Codex ligado nas Configurações.
- `⌘K`, e digite **agente**.
- O botão de agente novo, na barra do canvas.
- Com a voz configurada, `⌥C` e *"abre um agente"*.

`⌘T` abre um terminal no mesmo lugar, sem agente nenhum em cima dele. Veja
[o painel do terminal](painel-terminal).

## O nome

Cada agente nasce com um nome próprio. É por ele que a voz, o `⌘K` e os outros agentes o endereçam,
e é o nome que aparece no [elenco](painel-elenco) depois que ele for dispensado.

## A primeira tarefa

Digite no painel como você digitaria no seu terminal. *"Me explique o que este projeto faz"* é um
pedido curto e verificável: ele lê os arquivos, responde, e você vê o painel mudar de estado no
caminho.

## O estado do painel

O indicador de cada painel tem cinco estados: **parado**, **trabalhando**, **esperando você**,
**caído** e **encerrado**.

**Caído** é o turno encerrado por erro, e **parado** é o turno concluído. A retomada automática do
agente caído se configura em [ajustes dos agentes](ajustes-agentes).

`⌥F` vira todos os painéis de uma vez e mostra o resumo de cada agente: a missão, o que ele fez e há
quanto tempo. Veja [saber o que fazem](saber-o-que-fazem).

## Quando ele não abre

O painel diz o que está faltando: o programa de agente não instalado, ou o app ainda procurando onde
ele mora. Para o resto, veja [quando algo não funciona](quando-algo-nao-funciona).
