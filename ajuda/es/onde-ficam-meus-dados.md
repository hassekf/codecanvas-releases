---
slug: onde-ficam-meus-dados
titulo: Dónde están tus datos
resumo: Qué guarda CanvasCode en tu máquina, dónde guarda los secretos, y qué sale de aquí, hacia dónde y por qué.
area: conta
nivel: basico
---

CanvasCode no tiene cuenta ni servidor propio de datos. Lo que sale de tu máquina sale porque una
función que usaste necesita un servicio de fuera, y esta página dice cuál, y qué.

## En tu disco

En `~/Library/Application Support/codeCanvas`:

- **`canvases.json`**: los proyectos, los paneles con posición y tamaño, las áreas de trabajo, el
  tema, el fondo, las disposiciones guardadas y el registro de los agentes que vivieron en cada
  proyecto.
- **`tarefas/` y `notas/`**: tareas y notas, un archivo por proyecto.
- **`imagens/`**: las imágenes generadas y pegadas, una carpeta por proyecto, con el pedido que creó
  cada imagen generada.
- **`fundos/`**: copia de cada fondo de pantalla que elegiste o pediste.
- **`modulos/` y `modulos-dados/`**: los módulos que creaste y lo que guardan.
- **`voz/`**: el extracto de uso de la voz, un archivo por día, y el diario técnico que registra cada
  conexión del micrófono.
- **`custos/`**: el registro de lo que gastaron la voz y la conversación.
- **`Recados/`**: los recados ya abiertos, los que enviaste y la cola de confirmación.
- **`entregas/`**: lo que un agente escribe para otro cuando uno de ellos delega una tarea.
- **`backups/`**: copias automáticas del `canvases.json`, de las preferencias, de las tareas y de las
  notas.
- **`crashes.json` y `quedas.jsonl`**: el registro de los cierres inesperados de la app y de las
  caídas de agentes.

Las **grabaciones de pantalla** van a `~/Movies/codeCanvas`. Las **preferencias** de la app quedan
donde macOS guarda las preferencias de una app.

Nada de esto se envía a ningún sitio, y los backups tampoco salen de la máquina.

## Los secretos

Están en el **Llavero de macOS**, nunca en un archivo de texto:

- tu clave de OpenAI;
- tu clave de licencia y el token que devuelve la activación;
- los tokens de las integraciones que conectes, uno por proyecto;
- los secretos que registres en los servidores MCP;
- las claves privadas de este Mac para los recados.

El campo de la clave de OpenAI muestra si está configurada, nunca la clave. Los backups no llevan
ninguno de estos elementos.

## La conversación de los agentes

Es del programa de agente, no de la app, y vive en la carpeta de ese programa: `~/.claude`, `~/.codex`
y equivalentes, o la carpeta de la cuenta que elegiste para ese proyecto. CanvasCode guarda solo la
**clave** de cada conversación, que es lo que permite recuperar un agente con toda su memoria.

Un agente recuperado en otra cuenta no encuentra la conversación que tuvo en la primera. Ver
[cuentas y perfiles](contas-e-perfis).

## Qué sale de aquí

### Los agentes

Lo que le mandas a un agente va al servicio de ese agente, igual que iría si ejecutaras el mismo
programa en tu terminal. La app no media esa conversación y no guarda copia de ella.

### La voz, el comando y las imágenes

Todo esto usa tu clave de OpenAI, y nada de ello ocurre sin ella.

- **La conversación con la asistente** manda y recibe **audio**.
- **La voz con la que habla** manda el texto que se va a leer.
- **El modo comando** manda **texto**: la frase transcrita, más los nombres de los agentes vivos, de
  los proyectos abiertos, de los temas y de los CLIs activados. Sin clave, usa el modelo que corre en
  tu Mac.
- **Generar una imagen** y **pedir un fondo de pantalla** mandan tu pedido. El "buscar" del fondo
  busca en la web por el servicio de OpenAI.

El **dictado** no sale de la máquina con ninguno de los dos motores: el del sistema transcribe por
macOS, y Parakeet corre en tu Mac después de descargar el modelo. Ver [dictado](ditado) y
[cuánto cuesta](quanto-custa).

### La agenda

La agenda solo se lee si la activas en **Ajustes → Integraciones**. Activada, cinco elementos de cada
evento pueden mandarse a la asistente junto con la conversación, y los eliges uno a uno: título,
lugar, descripción y orden del día, participantes y enlace de la llamada. Todos nacen activados.
También eliges qué agendas del Calendario entran. Ver [agenda y reuniones](agenda-e-reunioes).

### Los recados

Un recado sale de este Mac cifrado de extremo a extremo, con claves que solo existen en el Llavero de
aquí y en el del destinatario. El servidor entrega y olvida el sobre; la copia que queda es la de tu
disco. Ver [el panel de recados](painel-recados).

### Las integraciones de empresa

Jira y Confluence hablan con el servidor de tu organización, y solo cuando lo pides. Ver
[Jira y Confluence](jira-e-confluence).

### La licencia

Activar, revalidar y liberar el Mac mandan tu clave de licencia, un **código derivado del
identificador de este Mac**, y el nombre del Mac tal como lo conoce macOS. La activación manda además
la versión de la app y la de macOS. El código del Mac está revuelto y no es reversible. Ver
[licencia](licenca).

### Los informes de fallo

Cuando la app se cierra de golpe, macOS graba un informe técnico en tu disco. El interruptor **Enviar
informes de fallo y de reanudación fallida**, en **Ajustes → Diagnóstico**, decide si se envía; la
app pregunta la primera vez que haya algo que mandar.

- El informe lleva el rastro de dónde tropezó la app, su versión y la de macOS. **No** lleva tu
  código ni tus archivos.
- El mismo interruptor cubre el fallo en que un agente vuelve sin su conversación. Ahí van recuentos,
  fechas y los identificadores de las sesiones; la ruta de tu proyecto se convierte en un código, y
  el nombre de tus cuentas no sale de aquí.
- Apagado, no se envía nada. La lista debajo del interruptor muestra lo ya recogido y lo que queda
  por mandar, con un botón de enviar en cada fila.

### Las actualizaciones

La app consulta al servidor de actualizaciones si hay versión nueva y la descarga cuando la hay. Cada
actualización está firmada, y la app rechaza cualquier archivo cuya firma no cuadre. Ver
[actualizaciones](atualizacoes).

## Los agentes hablan con el lienzo sin salir de la máquina

Cuando un agente abre un panel, lee tus tareas o fotografía el navegador, habla con un servidor que la
app levanta dentro de tu Mac. Escucha solo en loopback, y exige un secreto que nace en cada ejecución
de la app y se entrega a cada agente que nace aquí.

## Llevárselo todo

La carpeta de la app es una carpeta común: puedes copiarla, guardarla o borrarla desde el Finder.
Fuera de ella quedan los secretos en el Llavero, las grabaciones en `~/Movies/codeCanvas` y las
conversaciones de los agentes, que son de su propio programa.
