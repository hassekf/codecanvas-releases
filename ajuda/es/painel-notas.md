---
slug: painel-notas
titulo: El panel de notas
resumo: Un bloque de texto por ventana: cambiar de nota, crear, renombrar, borrar, y lo que los agentes escriben aquí.
area: paineis
nivel: basico
---

Ábrelo con `⌘K` y `nova nota`. Cada panel muestra una nota, y las notas pertenecen al lienzo.

El panel no tiene botón de guardar: el texto va al disco medio segundo después de que dejas de
escribir, y también cuando la ventana sale de escena.

## La cabecera

- **El nombre de la nota**: abre el menú con todas las notas de este lienzo, la tocada más
  recientemente primero. Elegir una cambia lo que muestra esta ventana.
- **Nueva nota** (en el menú y en el botón de la derecha): vacía el área de escritura. La nota nace
  en el primer carácter escrito; abrir y cerrar sin escribir no deja nada en el disco.
- **Nueva ventana de notas**: abre otro panel, para tener dos notas a la vista a la vez.
- **Renombrar…**: cambia el nombre. Enter y hacer clic fuera confirman, Esc cancela, y un nombre
  vacío devuelve la nota a su título automático.
- **Borrar**: manda la nota a la papelera. La ventana pasa a mostrar la nota tocada más
  recientemente.
- **El nombre del lado derecho**: aparece cuando la última mano que escribió ahí no fue la tuya.

## El nombre de una nota

Una nota no necesita nombre. Sin bautizar, se presenta por la primera línea de su propio texto,
cortada en 42 caracteres, y una nota sin texto aparece como "Nota vazia". Es por ese nombre que `⌘K`
la encuentra: escribe el nombre de una nota y abre una ventana en ella. Ve
[búsqueda y comandos](busca-e-comandos).

## La papelera

- **Papelera**, en el menú de la cabecera: aparece cuando hay algo borrado, con el recuento al lado.
- **Restaurar**: devuelve esa nota a la lista y la muestra en la ventana.
- **Vaciar la papelera**: borra definitivamente lo que hay dentro.

Ninguna herramienta de voz o de agente borra una nota.

## Quién más escribe aquí

Nina, por voz, y los agentes de este lienzo.

- **Una nota creada por un agente**: se abre en un panel en tu pantalla, con su nombre.
- **Una nota que ya existe**: el agente añade al final, nunca reescribe ni borra lo que había.
  También puede renombrarla.
- **Leer**: el agente lee los títulos, o el texto entero de una nota que menciones.

Ve [el agente usa tus listas](o-agente-usa-suas-listas).

En **Configuración → Herramientas**, desactivar el grupo **Notas** quita el control por voz y no
cambia nada en el panel.

Para lo que falta hacer, en vez de texto a guardar, usa [el panel de tareas](painel-tarefas).
