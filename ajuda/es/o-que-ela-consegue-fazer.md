---
slug: o-que-ela-consegue-fazer
titulo: Lo que se puede pedir
resumo: El repertorio de Nina por tema: la frase que dices, y lo que pasa en el lienzo.
area: nina
nivel: basico
---

Todo lo de aquí vale en las tres formas de mandar: [la conversación por voz](falar-com-a-nina) (⌥C),
[el modo comando](o-modo-comando) (⌥X) y [la conversación escrita](a-nina-por-texto) (⌘J). Los grupos
de herramientas se apagan en **Ajustes → Herramientas**, y cada uno muestra ahí cuántos tokens cuesta
por intercambio.

**Las frases de ejemplo de abajo se quedan en portugués, a propósito.** Las órdenes de voz se
interpretan en portugués, así que un ejemplo traducido sería una frase que no funciona. Dilas tal
como están escritas; la columna de al lado, en español, dice lo que pasa.

## Agentes

| Dices | Qué pasa |
|---|---|
| *"abre um agente"* · *"sobe dois agentes"* | Nacen en el lienzo, ya con nombre |
| *"cria um agente do Codex"* | Lo mismo, en la CLI que nombres |
| *"chama o Hermes de volta"* | El agente despedido vuelve con la conversación entera |
| *"ei Freya, roda os testes"* | La tarea va a Freya, tal como la dijiste |
| *"manda alguém investigar o build lento"* | Ella elige un agente libre, o crea uno |
| *"fecha a Freya"* · *"dispensa o Apolo"* | El panel sale de la pantalla y la memoria queda guardada |
| *"manda o Apolo continuar"* | El agente caído retoma desde donde paró |
| *"só quando o Claude voltar ao ar"* | La retomada espera a que el proveedor salga de la caída |
| *"deixa o Apolo falar com a Gerda do backend"* | Abre la conversación entre agentes de proyectos distintos |

Hablar con un agente no crea a nadie: un agente despedido vuelve por su nombre, con la conversación
entera. Las peticiones que exigen trabajo real (buscar, comparar, escribir código) se entregan a un
agente.

## Saber qué está pasando

| Dices | Qué pasa |
|---|---|
| *"como estamos?"* | Ella cuenta en qué anda cada agente |
| *"quais agentes existem?"* | Los que están en la pantalla y los guardados |
| *"quem está trabalhando agora?"* | Solo los que están en una tarea |
| *"o que o Apolo andou fazendo?"* | La tarea de Apolo, lo que hizo y lo último que respondió |
| *"quem foi que mexeu no pagamento?"* | Busca el tema en el historial de todos, incluidos los despedidos |
| *"mostra o status"* · *"esconde o status"* | Voltea y desvoltea los paneles |
| *"o que ele perguntou?"* · *"quais são as opções?"* | Lee la pregunta pendiente de un agente |
| *"a segunda"* · *"usa o que já está no docker compose"* | Responde esa pregunta, por la opción o con un texto tuyo |

"Mostra" cambia la pantalla; "me diz" produce una frase hablada. Cuando tu respuesta no coincide con
ninguna opción de la pregunta de un agente, ella repite la pregunta en lugar de elegir por ti.

## Paneles y disposición

| Dices | Qué pasa |
|---|---|
| *"abre o git"* · *"abre um terminal"* · *"abre a mídia"* | El panel nace en el lienzo |
| *"abre o browser no localhost:3000"* | Un navegador ya en esa dirección |
| *"me mostra o README"* | El archivo se abre en un panel |
| *"fecha o browser"* · *"fecha os agentes"* · *"fecha tudo"* | Cierra por nombre, por tipo, o el área entera |
| *"coloca o browser em foco"* · *"tira o foco"* | Destaca un panel y devuelve los demás a la rejilla |
| *"me leva até a Gerda"* | La cámara va hasta Gerda, cambiando de proyecto y de área si hace falta |
| *"organiza as janelas"* · *"põe em duas colunas"* | Ordena el lienzo, o cambia la disposición de la rejilla |
| *"salva esse arranjo como revisão de PR"* | Guarda la disposición con ese nombre |
| *"volta pro arranjo de pareamento"* | Restaura una disposición guardada, sin abrir ni cerrar ningún panel |

Cerrar cubre un panel por su nombre, varios, todos los de un tipo o el lienzo entero. Ver
[ordenar solo](organizar-sozinho).

## Proyectos y áreas

| Dices | Qué pasa |
|---|---|
| *"muda pro projeto platform"* | Cambia de lienzo |
| *"cria um canvas em /Users/eu/www/site"* | Crea un proyecto en esa carpeta |
| *"cria uma área pro front"* | Nace una pestaña nueva en este lienzo |
| *"vai pra área do back"* · *"próxima área"* | Cambia de pestaña |
| *"manda o Marshall pra área do back"* | El agente va vivo, en medio de lo que esté haciendo |

Un proyecto es otra carpeta con otro elenco; un área es otra pestaña del mismo proyecto. Ver
[áreas de trabajo](areas-de-trabalho) y [varios lienzos](varios-canvases).

## Tareas

| Dices | Qué pasa |
|---|---|
| *"anota aí que eu preciso arrumar o login"* | Crea la tarea |
| *"bota na lista: entregar o relatório sexta"* | La crea con plazo |
| *"o que falta neste projeto?"* · *"o que eu tenho pra hoje?"* | Lee lo que está abierto |
| *"marca a três como feita"* | Cambia el estado de la tarea 3 |
| *"muda o prazo da dois pra amanhã"* | La reprograma |
| *"comenta na do relatório que já testei"* | Escribe un comentario firmado |
| *"tira aquela do login da lista"* | La manda a la papelera |

"Já fiz" la marca como hecha; borrar solo ocurre cuando lo pides, y la tarea va a la papelera del
[panel de tareas](painel-tarefas).

## Notas

| Dices | Qué pasa |
|---|---|
| *"guarda esse endereço numa nota"* | Crea una nota |
| *"lê a nota do deploy"* | Ella lee el texto entero de esa nota |
| *"adiciona na nota do deploy que a porta é 8080"* | Añade al final, sin reescribir lo que había |

Ella crea, añade al final y renombra. Borrar una nota es solo desde [el panel](painel-notas).

## Recados

| Dices | Qué pasa |
|---|---|
| *"quem são meus contatos?"* | Lista a quienes ya añadiste |
| *"o que chegou de recado?"* | Lee los no leídos |
| *"avisa o Pedro que o deploy saiu"* | Manda un recado nuevo |
| *"responde pra ela que eu vejo amanhã"* | Responde al último que llegó |

Un recado va a otra persona, en otro ordenador. Ver [los recados](painel-recados).

## Repositorio e issues

| Dices | Qué pasa |
|---|---|
| *"como está o git?"* | La rama, lo que cambió y los últimos commits |
| *"o que mudou e ainda não foi commitado?"* | Los archivos sucios, con quién tocó cada uno |
| *"quais PRs estão abertas?"* · *"quais esperam a minha revisão?"* | Lista las pull requests |
| *"aprova a 42"* | Publica la aprobación en GitHub |
| *"comenta na 42 que falta o teste"* | Comenta sin aprobar |
| *"quais issues estão abertas?"* | Lista las issues |
| *"cria um bug com esse erro do console"* | Abre una issue |
| *"renomeia a issue 12"* · *"fecha a 12"* · *"reabre a 12"* | Actúa sobre esa issue |
| *"pega a primeira issue e começa"* | Abre un agente con la issue como tarea |
| *"manda esse bug pro Hermes"* | Entrega la issue a un agente ya abierto |

La lectura del repositorio dice qué agente tocó cada archivo. Ver [el panel de Git](painel-git).

## Jira y Confluence

| Dices | Qué pasa |
|---|---|
| *"o que tem no board?"* · *"o que tá em andamento?"* | Lee el tablero del proyecto conectado |
| *"cria uma tarefa pra revisar o login"* | Crea una tarjeta en Jira |
| *"move a PROJ-12 pra pronto"* | Mueve la tarjeta de columna |
| *"o que o Confluence diz sobre o fluxo de pagamento?"* | Busca en la base de documentación |

Cada proyecto habla con su propia cuenta. Ver [Jira y Confluence](jira-e-confluence).

## Skills y MCP

| Dices | Qué pasa |
|---|---|
| *"quais skills este projeto tem?"* | Lista las skills que este lienzo tiene a mano |
| *"desativa a skill de revisão aqui"* | La apaga solo en este proyecto |
| *"procura uma skill de testes"* · *"instala essa aí"* | Busca en el registro público e instala |
| *"quais MCPs estão ligados?"* · *"procura um MCP de Postgres"* | Lo mismo, para servidores de herramientas |

Instalar deja correr código de terceros en tus agentes, así que esa petición pasa por una
confirmación tuya. Ver [skills y MCP](skills-e-mcp).

## Apariencia e imágenes

| Dices | Qué pasa |
|---|---|
| *"troca o tema pra forja"* · *"deixa em ameixa"* | Cambia el tema de este proyecto |
| *"põe um fundo de floresta"* | Pinta un papel tapiz nuevo |
| *"procura outro"* | Lo cambia por el siguiente candidato, sin repetir la descripción |
| *"tira o fundo"* | Devuelve el paisaje del tema |
| *"gera uma imagem de um gato astronauta"* | La imagen nace en el lienzo y va a la galería |
| *"cria três ilustrações de uma floresta"* | Lo mismo, en la cantidad que pidas |
| *"quantas imagens tem no canvas?"* | Ella cuenta lo que está pegado ahí |

El fondo es el papel tapiz; una imagen generada aparece en el lienzo y se queda en
[la galería](painel-galeria). Las dos tardan un poco, y la app avisa cuando están listas. Ver
[apariencia](aparencia).

## Medios, cámara y grabación

| Dices | Qué pasa |
|---|---|
| *"põe pra tocar"* · *"pausa aí"* | Comanda lo que ya está en el panel de medios |
| *"muda pra música"* | Cambia entre vídeo y música |
| *"minimiza o vídeo, quero só o áudio"* | Lo encoge en una cápsula, con el sonido siguiendo |
| *"modo cinema"* | Esconde la página y deja solo el vídeo |
| *"abre a webcam"* · *"espelha a imagem"* · *"usa a câmera do iPhone"* | Abre y ajusta la cámara |
| *"começa a gravar"* · *"pausa a gravação"* · *"para de gravar"* | Comanda la grabación de pantalla |
| *"deixa a janela em vertical"* · *"põe em paisagem"* | Redimensiona la ventana de la app para grabar |

Ella comanda lo que ya está sonando; elegir el vídeo es una petición que va a un agente. Ver
[el panel de medios](painel-midia), [la cámara](painel-webcam-e-avatar) y
[la grabación](painel-gravacao).

## Agenda y reuniones

| Dices | Qué pasa |
|---|---|
| *"o que eu tenho hoje?"* · *"qual a próxima reunião?"* | Lee tu agenda |
| *"do que é a reunião das três?"* · *"quem vai estar nela?"* | Detalla una cita |
| *"entra na reunião"* · *"abre o Meet"* | Abre la llamada y enciende el modo reunión |
| *"fica quieta um pouco"* | Enciende el modo reunión sin ninguna reunión |
| *"acabou a reunião"* | Apaga el modo reunión |

Ella lee el calendario y entra en la llamada. No crea, no mueve y no cancela citas. Ver
[agenda y reuniones](agenda-e-reunioes).

## Un dictado que fue al agente equivocado

| Dices | Qué pasa |
|---|---|
| *"aquilo da migração, joga pro Hermes"* | El texto que ya dictaste va a otro agente |
| *"mandei errado, reenvia o último pro Apolo"* | Lo mismo, con el último dictado |

Se reaprovecha el texto original; no hace falta repetir la frase. Ver [dictado](ditado).

## Cerrar

*"pode dormir"*, *"tchau"*, *"valeu"* y *"chega"* cierran la conversación por voz. Los agentes siguen
trabajando.
