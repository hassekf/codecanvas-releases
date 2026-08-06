---
slug: painel-iniciativas
titulo: El panel de Iniciativas
resumo: Las tres pantallas del panel, qué hace cada botón de una ejecución, y qué pasa cuando se detiene en ti.
area: iniciativas
nivel: avancado
---

Ábrelo con `⌘K` e **iniciativas**, **runs**, **ejecuciones**, **workflow**, **pipeline**, **pasos** o
**puerta**.

Una Iniciativa es un proceso escrito en un archivo de `.codecanvas/iniciativas/` del repositorio. Una
**ejecución** es una corrida de ese proceso.

## Cuando no existe ninguna

El panel muestra lo que encontró en el repositorio sin ningún agente (comandos, scripts de
validación, ejecuciones antiguas) y dos botones. En los dos eliges el agente, y la conversación pasa
en el panel de él:

- **Escribirla desde cero, conversando**: el agente recibe el aviso de que van a diseñar un proceso.
- **Leer el proyecto y proponer**: el agente recibe además lo que el panel encontró, y propone.

## La lista

- **Todas**, **En marcha**, **Te esperan**, **Esperan fuera**, **Completadas**: filtran las
  ejecuciones. Cada uno trae su cuenta.
- **El menú de Iniciativa**: restringe la lista a una de ellas. Solo aparece con más de una Iniciativa
  en el proyecto.
- **Nueva iniciativa**: elige un agente y abre la conversación para escribir una.
- **Nueva ejecución**, en la línea de una Iniciativa: empieza una corrida.
- **Archivar**, en la línea de una ejecución terminada: la saca de la lista sin borrar su carpeta.
- El botón a la derecha de cada ejecución cambia con su situación: **Responder**, **Resolver**, **Leer
  qué se atascó**, **Reanudar**, **Ver qué falta**, **Ver el resultado**.

Una Iniciativa que vive en un [worktree](worktrees-e-isolamento) aparece con la rama al lado, y sus
ejecuciones pasan ahí dentro.

Un archivo que la app no pudo leer **aparece en la lista igual**, marcado, y su pantalla lista cada
rechazo con el campo y el motivo. Su menú ofrece **Ver los problemas**, **Pedirle a un agente que lo
arregle** y **Abrir el archivo**.

## La pantalla de una Iniciativa

Muestra los pasos en orden, qué recibe y qué produce cada uno, quién lo ejecuta (un comando o un
agente), las puertas, las revisiones, el tope de vueltas de cada ruta y qué pide la Iniciativa para
empezar.

- **Nueva ejecución**: empieza una corrida.
- **Editar con un agente**: manda el archivo y lo que quieres cambiar al agente que elijas.
- **Ver los orígenes**: los archivos del proyecto de los que salió la Iniciativa, cada uno marcado
  como **apunta** (la ejecución lee la versión de ahora) o **copia** (la ejecución usa la versión
  guardada en la Iniciativa).
- **Ver qué cambió**: aparece cuando un archivo de origen cambió después de que la Iniciativa fue
  escrita. **Releer con el agente** le manda el archivo, qué cambió en él y la Iniciativa que salió
  de ahí.
- **Archivar las completadas** y **Eliminar la Iniciativa**, en el menú: eliminar manda el archivo
  `.json` a la papelera; las ejecuciones del historial y los archivos del proyecto se quedan donde
  están.

## Empezar una ejecución

**Nueva ejecución** pide lo que la Iniciativa declaró necesitar: una fuente (un enlace, una clave de
tarjeta, un archivo), un texto, una lista de preguntas, la salida de otra ejecución, o nada. Sin esa
entrada, el botón de empezar no está disponible.

En la misma pantalla:

- **El nombre de la ejecución**: sugerido a partir de lo que diste, editable. La pantalla dice si el
  nombre ya existe, y en ese caso le agrega un sufijo.
- **Con qué herramienta**: el proveedor de los agentes de los pasos que no fijan el suyo.
- **Sola hasta que te necesite**: encadena los pasos y solo se detiene en las puertas que te piden, o
  si una puerta se atasca.
- **Paso a paso**: se detiene después de cada paso y espera que la hagas seguir.
- **Dónde pasa el código**: aísla en un worktree propio los pasos que escriben código, con la rama y
  la carpeta escritas en la pantalla. Las instrucciones de los agentes vienen de este lienzo o de
  [configuración de los agentes](ajustes-agentes), y **personalizar** las cambia solo para esta
  ejecución.
- **Empezar la ejecución**.

## Mientras la ejecución avanza

- **Cada paso** nace con un agente propio, sin panel. Al hacer clic en el paso se abre su panel;
  minimizarlo lo esconde de nuevo.
- **Ver el panel del agente**: lo mismo, desde el botón.
- **Pausar tras este paso** y **Dejar que corra hasta el final**: cambian el modo de una ejecución en
  marcha.
- Quien ejecuta la puerta de un paso es la app, después de que el agente dice que terminó. Si la
  puerta rechaza, el trabajo vuelve al agente con el motivo, hasta el tope de vueltas de esa ruta.
- Si el agente de un paso muere, la app pone otro en su lugar hasta dos veces. A la tercera, la
  ejecución se detiene y dice que el problema fue la caída.
- Si cierras la app con una ejecución en marcha, vuelve marcada como interrumpida, y **Reanudar desde
  aquí** la enciende de nuevo.
- **Terminar la ejecución**, en el menú: interrumpe lo que esté pasando. Los artefactos ya escritos,
  el worktree y los commits se quedan; una ejecución terminada no vuelve a andar.

## Cuando la ejecución se detiene en ti

- **Firma**: la pantalla muestra lo que la Iniciativa mandó mostrar (el documento, la vista previa de
  lo que va a pasar fuera del lienzo, o el pedido escrito). El botón de aprobar lleva la etiqueta que
  la Iniciativa escribió. **Devolver con un comentario** abre el campo y devuelve el paso con tu
  texto; devolverlo sin escribir nada no es posible.
- **El agente preguntó**: la pregunta salió a mitad del paso y no estaba en el proceso. Responder no
  aprueba nada ni avanza el paso; el texto llega al agente en su próximo turno.
- **Espera a alguien de fuera**: la pantalla dice qué está esperando el paso. Puedes soltar el
  archivo, pegar un enlace o escribir lo que llegó, y **Ya llegó, puede seguir** lo libera. **Copiar
  la petición** copia lo que falta, para que se lo mandes a quien tenga la pelota.
- **Se atascó**: se acabó el tope de vueltas, o el comando de la puerta no estaba donde la Iniciativa
  dijo. Los botones son **Intentar la puerta de nuevo**, **Seguir sin que pase la puerta**, **Dar 3
  vueltas más** y **3 más, con un agente nuevo**. Cuando el comando de la puerta no existe, no se
  gasta ninguna vuelta y la pantalla dice dónde buscó la app.
- **Paso a paso**: al final de cada paso la pantalla muestra quién haría el siguiente, qué entra y qué
  sale, y espera el botón.

## Cuando termina

La pantalla de la ejecución muestra los artefactos, dónde quedaron (la carpeta o la rama), cuántas
firmas tuyas llevó y cómo pasó cada puerta. **Ejecutar de nuevo** empieza otra ejecución de la misma
Iniciativa. Lo que la Iniciativa declaró hacer con el resultado se ofrece como botón, nunca se hace
solo.

## Enterarte con el panel cerrado

- **La píldora de la barra de comando**: cuenta las ejecuciones vivas del proyecto y abre la lista de
  ellas, con la ejecución y el paso de cada una. Cuenta lo que está vivo, no lo que está trabajando.
  Por defecto queda siempre visible y sirve de acceso directo; **Ocultar las Iniciativas cuando no hay
  nada pendiente**, en Configuración → Interfaz, hace que solo aparezca durante una ejecución.
- **Los avisos**: una ejecución avisa cuando termina, cuando se detiene esperándote, cuando hace una
  pregunta, cuando se atasca y cuando llega lo que esperaba de fuera. Pasar de un paso a otro no
  avisa. Al hacer clic en el aviso se abre esa ejecución. Con el panel de la ejecución a la vista, el
  aviso no se lee en voz alta. Los interruptores de sonido, voz y notificación de macOS son los de
  [avisos y sonidos](avisos-e-sons).

## Limitaciones

- **Editar la Iniciativa con una ejecución en marcha cambia la corrida en curso**. La pantalla de
la ejecución avisa cuando eso pasó.
- **Una Iniciativa está hecha de los comandos y scripts de ese repositorio**, y por eso no es
  reutilizable en otro proyecto.
