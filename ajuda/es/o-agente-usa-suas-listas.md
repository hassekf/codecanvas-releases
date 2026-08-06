---
slug: o-agente-usa-suas-listas
titulo: El agente usa tus listas
resumo: Qué lee y escribe un agente en tus tareas, tus notas y tus mensajes, y qué no puede hacer en ellas.
area: agentes-fazem
nivel: basico
---

## Qué pedir

- *"Mira en la lista si esto ya está anotado antes de empezar."*
- *"Coge la próxima tarea y trabaja en ella."*
- *"Márcala como hecha y comenta qué hiciste."*
- *"Anota en la nota de las claves el token nuevo del servidor de pruebas."*
- *"Responde el mensaje de Bruno contándole que ya está en línea."*

## Las tareas

Ver [el panel de tareas](painel-tarefas).

- **Leer la lista**: lo que falta, con plazo, estado y quién tocó cada tarea. Las completadas solo
  aparecen si el agente las pide.
- **Crear**: texto y, cuando tú digas uno, plazo en `AAAA-MM-DD`, con hora opcional.
- **Actualizar**: estado (abierta, haciendo, hecha), comentario, texto y plazo. Solo se envía lo que
  cambió.
- **Borrar**: la tarea va a la papelera, desde donde la restauras en el panel. El historial registra
  que fue el agente quien la borró.

Tres cosas que la lista no muestra:

- **Cada comentario va firmado con el nombre del agente que lo escribió.** No elige la firma, no
  firma como otro agente y no firma como tú.
- **Completar y borrar son cosas distintas.** "Ya está hecho" es el estado `hecha`, con un comentario
  de lo que se hizo. Borrar es solo cuando tú lo pides.
- Los agentes tienen instrucción de no reorganizar la lista, no decidir prioridades y no usarla como
  cuaderno propio.

## Las notas

Ver [el panel de notas](painel-notas).

- **Leer**: sin señalar cuál, el agente recibe los títulos. Señalando el título o un fragmento,
  recibe el texto entero de esa nota.
- **Crear**: con título, o sin él, y entonces la primera línea del texto se convierte en el nombre.
- **Actualizar**: añade texto al final, en una línea nueva, o renombra la nota.

**No existe ninguna vía para que un agente reescriba o borre lo que hay en una nota.** Borrar una
nota es un gesto tuyo, en el panel.

## Los mensajes

Los mensajes van a otra persona, en otro ordenador. Ver [el panel de mensajes](painel-recados).

- **Listar contactos**: a quién ya has añadido, y quién mandó un mensaje sin leer. La lista viene
  numerada.
- **Leer los mensajes**: sin señalar de quién, los no leídos. **Leer por esta vía los marca como
  leídos**, y el panel deja de mostrarlos como nuevos. Los adjuntos no vienen en el texto: se citan
  por su nombre, y quien los abre eres tú.
- **Responder** un mensaje que llegó, y **mandar** uno nuevo, con asunto y cuerpo.
- Un archivo puede ir con el mensaje: lo que viaja es el contenido, con un tope de 5 MB, y no la
  ruta.

Dos restricciones:

- Un agente solo manda mensajes a quien está en tus contactos. Nadie es localizable por búsqueda.
- **Quien nunca definió su propio nombre aparece como "sin nombre"**, y el número de la lista es la
  única forma de dirigirse a esa persona.
