---
slug: o-agente-e-o-git
titulo: El agente y el repositorio
resumo: Leer el estado del repositorio con la autoría de lo aún no confirmado, resolver issues y revisar pull requests de GitHub.
area: agentes-fazem
nivel: avancado
---

## Qué pedir

- *"Antes de tocar ese archivo, mira si hay alguien en él."*
- *"Dime qué falta por confirmar y qué ha estado tocando cada uno."*
- *"Coge el primer issue y resuélvelo. Comenta la causa y ciérralo cuando el arreglo esté
  confirmado."*
- *"¿Qué está esperando mi aprobación?"*
- *"Lee la PR 214 y dime si se puede aprobar."*

## Leer el repositorio

Un agente lee la rama actual, lo que aún no se ha confirmado y los últimos commits.

**Junto viene lo que git no tiene: qué agente escribió en cada archivo sucio.** El historial de git
solo conoce commits, y un archivo modificado y sin confirmar no tiene autor alguno. CanvasCode
registra la autoría de las ediciones hechas por los agentes de este lienzo, y la lectura señala
cuando dos agentes están en el mismo archivo.

- En ese caso no hay conflicto que git pueda detectar, porque nada se confirmó. Quien guarde último
  sobrescribe al otro.
- El mismo informe aparece para ti en [el panel de Git](painel-git).
- La salida para trabajo pesado en paralelo es cada agente en su propia copia del proyecto, en
  [worktrees y aislamiento](worktrees-e-isolamento).

## Los issues de GitHub

- **Listar** los issues abiertos: título, etiquetas y vista previa. Un filtro por etiqueta reduce la
  lista.
- **Leer un issue entero**, con el cuerpo completo, por su número.
- **Comentar**, **renombrar** y **cerrar**, con un comentario de cierre opcional.
- **Reabrir** un issue cerrado, con el motivo.

Los agentes tienen instrucción de comentar la causa real y no solo "resuelto", de renombrar el título
cuando solo describe el síntoma reportado, y de cerrar cuando el arreglo esté confirmado o cuando
concluyan que no era un error.

Los issues de Jira son otra cosa, y están en [el panel de Jira](painel-jira).

## Las pull requests

- **Listar** las PR abiertas: título, autor, rama, estado de la revisión y estado de la CI.
- **Leer una PR entera**, con la descripción y los archivos modificados, por su número.
- **Filtrar** por las que piden tu revisión.
- **Aprobar**, publicando una revisión de aprobación en GitHub, con comentario opcional.
- **Comentar**, sin aprobar.

**Pedir cambios y hacer merge no existen por aquí.** El merge sigue siendo tuyo, o del agente en su
terminal.

## Qué exige esto

Los issues y las pull requests vienen de GitHub por `gh`, con la sesión que ya está en la máquina. Si
falta alguna pieza, el agente recibe cuál de las tres es:

- `gh` no está instalado;
- `gh` está instalado y nadie ha iniciado sesión;
- el proyecto no tiene un remote de GitHub.

## Qué no existe por aquí

- Confirmar, crear ramas y hacer merge no son acciones del lienzo. El agente hace eso en su terminal,
  como lo haría fuera de la app.
- Un agente ve el repositorio del proyecto en el que vive, y solo ese.
