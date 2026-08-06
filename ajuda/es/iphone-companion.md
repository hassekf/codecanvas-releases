---
slug: iphone-companion
titulo: El iPhone emparejado
resumo: Emparejar el iPhone con este Mac, revocar un aparato, qué puedes hacer desde lejos y cuándo avisa el teléfono.
area: integracoes
nivel: basico
---

En **Configuración → Companion**. La app del teléfono se llama Canvas Companion, y forma parte del
plan **Team**.

## Emparejar

- **Emparejar un iPhone**: abre la ventana de la invitación. Trae un QR, para la cámara del teléfono, y
  la misma invitación escrita en un código de 6 caracteres, para dictar.
- **Copiar código**: pone el código en el portapapeles.
- **La invitación vale 5 minutos y un solo uso**, y muere cuando cierras esa ventana. Un reloj en la
  pantalla cuenta el tiempo restante.
- **Generar otra invitación**: sustituye a la invitación vencida. No se genera sola.
- Cuando el teléfono entra, la ventana cambia el QR por el nombre del aparato.

Si emparejaste escribiendo el código en vez de leer el QR, compara los caracteres de
**Este Mac** con los que aparecen en el teléfono. Esa comparación es la que prueba que la clave
guardada allí es la de este ordenador.

## La lista de aparatos

Cada línea trae el nombre del aparato, cuándo se emparejó, cuándo habló con este Mac por última vez y
la huella de su clave.

- **todavía no ha hablado con este Mac**: sustituye a la fecha de uso mientras el teléfono no se ha
  presentado.
- **chave trocada em <fecha>** (clave cambiada el): aparece cuando las claves de ese aparato
  cambiaron. Reinstalar la app del teléfono y que alguien robe la cuenta llegan aquí igual.
- **Revocar**: este Mac deja de aceptar ese aparato al instante, sin diálogo de confirmación. Para
  volver, hay que emparejarlo de nuevo, con el Mac delante.
- **Este Mac**: muestra el nombre de esta máquina y la huella de su clave. Cambiar de Mac exige
  emparejar los teléfonos otra vez.

Sin ningún aparato emparejado, nada de fuera habla con este Mac.

## Qué puedes hacer desde el teléfono

- **Ver los proyectos y los agentes de cada uno**, con el estado de ahora, lo último que pediste y
  los archivos que cada uno escribió.
- **Leer la conversación** de un agente, mensaje a mensaje.
- **Abrir un archivo** que el agente escribió.
- **Ver qué cambió** en la carpeta en la que trabaja el agente.
- **Responder la pregunta** que detuvo a un agente, eligiendo entre las opciones o escribiendo otra
  respuesta.
- **Mandar trabajo** a un agente. El envío normal pasa por la cola de la app: despierta al agente que
  duerme, espera un permiso abierto, y todavía se puede cancelar antes de que salga. El envío directo
  escribe en el terminal al instante, y el teléfono pide un gesto más para usarlo.
- **Interrumpir** a quien está en medio de algo, y **despedir** a quien ya terminó.
- **Abrir un proyecto** y cambiar el proyecto en foco aquí en el Mac.
- **Llamar a un agente nuevo**, y crear un área de trabajo.
- **Hablar con Nina**, que responde con lo que sabe de este lienzo.

Una petición de acción repetida no se ejecuta dos veces: tocar "intentar de nuevo" devuelve el
resultado de la primera.

## Cuándo avisa el teléfono

El teléfono toca el timbre en tres casos: un agente **se detuvo para preguntar** (el aviso trae el
enunciado de la pregunta), un agente **terminó** y un agente **se cayó**. El estado de rutina viaja a
la pantalla sin tocar el timbre.

## Los límites

- **El archivo tiene que estar en la carpeta en la que trabaja ese agente.** Nada fuera de ella es
  alcanzable, y un archivo grande llega cortado, con el aviso de que fue cortado.
- **La lista de lo que el agente escribió sale de las herramientas de escritura de la CLI.** Un
  archivo creado por un comando de terminal no entra en ella.
- **El Mac tiene que estar despierto.** Con él dormido, el teléfono recibe una respuesta que dice que
  el Mac no está listo.
- **Cada comando que llega pasa por la licencia y por la clave del aparato** antes de convertirse en
  acción, y lo que borra trabajo pide confirmación en el propio teléfono.
