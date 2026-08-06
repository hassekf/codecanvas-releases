---
slug: painel-tarefas
titulo: El panel de tareas
resumo: La lista del proyecto: anotar, cambiar de estado, poner plazo, el historial de cada línea y el aviso de vencimiento.
area: paineis
nivel: basico
---

Ábrelo con `⌘K` y `tarefas`. Hay un panel por lienzo, y la lista pertenece al lienzo: dos lienzos son
dos listas, aunque apunten a la misma carpeta.

## Anotar

- **El campo de arriba**: crea una tarea con el texto escrito. Enter y el botón **Anotar** hacen lo
  mismo. El plazo no se pide aquí.

## La lista

Tres secciones, en este orden: **Fazendo** (haciendo), **Abertas** (abiertas) y **Feitas** (hechas).

- **Fazendo** y **Abertas**: ordenadas por el plazo más cercano. Las que no tienen plazo van al
  final.
- **Feitas**: plegada, con el recuento al lado del título. Se abre al hacer clic, y también sola
  cuando completas una tarea. Dentro, la más reciente aparece primero.
- **El pie**: cuenta cuántas tareas están pendientes y cuántas vencieron.

Cada línea muestra el texto de la tarea, su número, el estado escrito, el plazo, quién la tocó por
última vez y cuántos comentarios tiene.

- **El número (`#3`)**: identifica la tarea para la voz y para los agentes. Es único en el lienzo y
  nunca se reutiliza, y reordenar la lista no renumera nada.
- **El nombre de quien la tocó por última vez**: aparece solo cuando no fuiste tú.
- **El último comentario**: queda visible en la línea cuando lo escribió un agente o Nina.
- **La barra del borde izquierdo**: marca la tarea cuyo plazo ya pasó. Una tarea hecha no recibe la
  barra, aunque el plazo haya vencido.

## Cambiar el estado

- **El círculo de la izquierda**: marca la tarea como hecha, y reabre la que ya está hecha. No pasa
  por "en curso".
- **Empezar** y **Pausar**: aparecen en la línea bajo el cursor. **Empezar** mueve la tarea abierta a
  en curso; **Pausar** devuelve la que está en curso a abierta.
- **El estado escrito en la línea**: es un menú, y lleva la tarea a cualquiera de los tres estados.
- **El menú contextual de la línea**: repite los tres estados, el plazo y **Borrar**.

## El plazo

El plazo es opcional. Desde el menú contextual de la línea, en **Plazo**:

- **Hoy**, **Mañana** y **La semana que viene**: fijan ese día a las 18h, y la línea muestra solo el
  día.
- **Quitar la fecha límite**: aparece solo cuando existe un plazo.

Un plazo con hora se define por voz ("entregar el viernes a las 17h") o por un agente. Sin hora, el
plazo cae a las 18h. El plazo vencido se escribe como "venceu às 13h" o "venceu 4 de agosto".

## El reverso de la línea

Hacer clic en la línea abre su reverso, y hacer clic de nuevo lo cierra.

- **Los comentarios**: todos, con el autor y cuándo se escribieron.
- **Comentar…**: añade un comentario tuyo.
- **Historial**: cada creación, cambio de estado, reescritura, plazo, comentario, borrado y
  restauración, con el nombre de quien lo hizo y cuándo. El nombre queda grabado ahí incluso después
  de que el agente sea despedido.

## La papelera

- **Borrar**: manda la tarea a la papelera, y el historial registra quién la borró. Un agente borra
  por la misma puerta.
- **Papelera**, en el pie: muestra lo borrado, con **Restaurar** en cada línea.
- **Vaciar**: borra definitivamente lo que está en la papelera. Ninguna herramienta de voz o de
  agente alcanza este botón.

## El aviso de plazo

Una tarea con plazo avisa tres veces: 1 hora antes, 30 minutos antes y al vencer. Cada marca avisa
una sola vez, y reabrir la app no repite lo ya dicho. Cuando llega más de una marca a la vez, solo se
dice la más urgente.

- **El aviso vale para todos los lienzos**, no solo el que tienes delante. Cuando la tarea es de otro
  proyecto, el aviso dice de cuál.
- **Hacer clic en el aviso**: cambia al lienzo de esa tarea y abre el panel de tareas.
- Activarlo, desactivarlo, callarlo y hacer que se lea en voz alta: [avisos y sonidos](avisos-e-sons).

## Quién más escribe aquí

Nina, por voz, y los agentes de este lienzo. Crean tareas, cambian el estado, comentan, reescriben el
texto, tocan el plazo y borran. Cada acción suya entra en el historial con el nombre de quien la
hizo, y su comentario es lo que aparece en la línea cuando completan algo. Ve
[el agente usa tus listas](o-agente-usa-suas-listas).

En **Configuración → Saludo**, **Buenos días al abrir** con **Hablar de las tareas** activado cuenta,
la primera vez que abres la app cada día, qué venció y qué vence hoy en tus listas.

Para texto que quieres guardar en vez de hacer, usa [el panel de notas](painel-notas).
