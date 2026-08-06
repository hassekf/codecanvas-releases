---
slug: painel-webcam-e-avatar
titulo: A câmera e o avatar
resumo: O painel com a imagem da sua câmera e o painel com o rosto da assistente: onde ficam os controles, quando a câmera desliga sozinha, e o que muda ao soltar da grade.
area: paineis
nivel: basico
---

Os dois abrem pelo `⌘K` (digite "webcam" ou "avatar").

## O painel de webcam

O corpo do painel é só a imagem. Os controles ficam no menu de clique direito, que abre tanto sobre
o cabeçalho quanto sobre a imagem:

- **Câmera**: escolhe a fonte da imagem. A lista traz as câmeras que o macOS enxerga no momento,
  incluindo a Continuity Camera e a Desk View do iPhone. **Padrão do sistema** deixa a escolha com o
  macOS. Conectar ou desconectar uma câmera atualiza a lista sem reabrir o painel.
- **Espelhar a imagem**: inverte a imagem na horizontal. A captura não é reiniciada.

A câmera e o espelho escolhidos ficam gravados no painel, e reabrir o app volta a eles. Se a câmera
escolhida desaparecer, o painel volta sozinho para a padrão do sistema em vez de ficar sem imagem.

### Um painel só no app inteiro

Existe **um** painel de webcam, não um por projeto. Abrir a webcam num canvas onde ela não está traz
o painel para lá, e a captura não é interrompida na mudança.

### Quando a câmera desliga sozinha

- **Durante uma reunião**: o painel libera a câmera para a chamada e a retoma quando a reunião
  termina. Veja [agenda e reuniões](agenda-e-reunioes).
- **Com a janela do app fechada**: o app segue rodando sem a janela, e a câmera é liberada junto com
  ela.

A câmera só volta a capturar quando nenhuma dessas razões está ativa.

### Solto da grade, sobra a imagem

Com o canvas em arranjo automático, o cabeçalho tem o botão **Soltar da grade**. Fora da grade e sem
seleção, o painel de webcam perde o cabeçalho e a borda: fica só a imagem. Nesse estado ele se move
arrastando a própria imagem, e um clique traz os controles de volta.

### A permissão

O macOS pede o acesso à câmera na primeira vez. Negado o acesso, o painel mostra **O acesso à câmera
está bloqueado** e o caminho para liberá-lo em Ajustes do Sistema. Autorizado, mas sem nenhuma
câmera disponível, ele mostra **Nenhuma câmera encontrada**. Veja
[as permissões que o macOS pede](permissoes-do-mac).

### Por voz

Abrir o painel, espelhar, tirar o espelho e trocar de câmera dizendo um trecho do nome dela ("usa a
do iPhone"). Com o painel fechado, o comando o abre antes de executar o resto.

## Com que câmera um painel novo nasce

Em **Configurações → Webcam**.

- **Câmera padrão**: a câmera com que um painel de webcam novo abre.
- **Espelhar a imagem por padrão**: se um painel novo já nasce com a imagem invertida.

Os dois valem para o **próximo** painel. Nenhum deles muda o painel já aberto, que guarda a escolha
feita nele.

## O painel do avatar

O rosto da assistente, desenhado em caracteres sobre um fundo animado. O desenho roda numa página
local dentro do app: nada dele sai da sua máquina.

O painel não tem controle nenhum. Quem o move é a conversa por voz:

- ao **abrir a conversa**, o rosto se condensa do fundo;
- enquanto **ela fala**, a boca acompanha o nível da voz que está saindo;
- ao **encerrar a conversa**, o rosto se dissolve e sobra o fundo.

O rosto adota a cor de destaque do tema do canvas em que o painel está, e muda junto quando você
troca de projeto. Veja [aparência](aparencia).

Como a webcam, o avatar é **um só no app inteiro** e fica sem cabeçalho nem borda quando solto da
grade.

Para o que a assistente faz além de aparecer, veja [falar com a Nina](falar-com-a-nina).
