---
slug: worktrees-e-isolamento
titulo: Cada agente en su copia
resumo: El aislamiento por worktree, el texto que instruye a los agentes, la barra de frentes y la entrega de un frente terminado.
area: agentes
nivel: avancado
---

## El aislamiento

En **Ajustes → Agentes → Aislamiento por worktree**, activado de forma predeterminada.

- **Aislamiento por worktree**: instruye a cada agente a crear su propio worktree del repositorio y a
  hacer commit en su propia rama antes de escribir cualquier archivo. Desactivado, todos los agentes
  escriben en el mismo directorio.
- **La instrucción vale para los próximos agentes.** Entra en el prompt de sistema al nacer el
  proceso, y ningún agente que ya esté en pie cambia de comportamiento cuando guardas.
- **Es una instrucción, no una traba de la app.** Un agente decide seguirla, y el protocolo se salta
  el worktree en las tareas de solo lectura y en los proyectos sin repositorio Git.

## El texto que leen los agentes

- **Personalizar instrucciones…**: abre el editor del protocolo, justo debajo del
  interruptor. Una vez editado, el botón pasa a decir **Editar instrucciones…**.
- **{nome}**: el marcador que se convierte en el identificador de cada agente, y por lo tanto en su
  rama y su carpeta. Sin él, el editor avisa y aun así permite guardar, y los agentes se
  disputan la misma rama.
- **Restaurar predeterminado**: repone el texto de fábrica en el editor, y queda no disponible cuando
  lo que hay ahí ya es el predeterminado.
- **Concluir** con el texto vacío, o idéntico al predeterminado, deshace la personalización: el
  proyecto vuelve a seguir el texto predeterminado en lugar de guardar una copia de él.

Cada proyecto puede discrepar del ajuste de la app, en **Editar el proyecto → Agentes → Aislamiento
por worktree**:

- **Seguir el ajuste global**, **Activado en este proyecto** o **Desactivado en este proyecto**.
- **Instrucciones propias de este proyecto**: aparece con el aislamiento activado y sustituye el
  texto global solo en este canvas.

## La barra de frentes

`⌘⇧F` abre y cierra la barra de la izquierda. La tecla se cambia en Ajustes → Atajos.

Cada sección es un área de trabajo, incluidas las que no están a la vista, y dentro de ella viene una
fila por agente.

- **La fila de un frente** trae el nombre del agente, las líneas sumadas y quitadas, la rama, la
  etapa y cuántos commits del destino todavía no ha visto. Al hacer clic, la cámara va hasta el
  agente.
- **La etiqueta "solo rama"** marca el trabajo que existe como rama y ya no tiene directorio.
- **Los agentes sin frente también aparecen**, con su estado actual: quien solo leyó código no tiene
  rama ni worktree.
- **La fila de arriba** es la base del canvas, con cuántos archivos están sin commit ahí.
- **El ojo del encabezado** muestra y oculta el asunto anotado por cada agente.
- **El botón de al lado** alterna entre la barra flotante y la barra anclada al lateral, con el
  canvas al lado. Nace flotante.
- **Los archivos en disputa** quedan al pie de la lista: los que más de un frente está tocando ahora,
  con commit o sin él.
- **El pie** cuenta cuántos frentes están listos para integrar y cuántos están en revisión, y el
  botón de al lado relee el repositorio desde cero, sin aprovechar lo que la barra ya sabía.
- **Un repositorio grande no se lee entero.** Las ramas con worktree entran siempre, y del resto
  entran las más recientes. La barra dice cuántas quedaron fuera.
- **El menú contextual de una fila** lleva hasta el agente, o trae un agente a un worktree sin dueño,
  y copia la ruta del worktree, el nombre de la rama, o abre la carpeta en el Finder.

## Lo que la barra lista

En **Ajustes → Interfaz → Barra de frentes**.

- **Mostrar ramas sin worktree**, activado: también aparecen las ramas cuyo directorio de trabajo ya
  fue eliminado. Desactivado, una rama en ese estado queda invisible.
- **Mostrar los ya integrados**, desactivado: los frentes que ya están enteros en la base salen de la
  lista.
- **Ocultar las pestañas de área cuando esté anclada**, desactivado: las pestañas de arriba
  desaparecen y la barra pasa a cambiar de área, renombrar y crear. Solo funciona con la barra
  anclada, y queda no disponible mientras esté flotando.
- **Agrupar los agentes en pestañas**: en un área con más de un agente, comparten un panel con
  pestañas arriba. El menú contextual de cada área puede decidir por su cuenta.

## Entregar un frente

El botón de entrega aparece en la fila de los frentes listos, publicados o en revisión, y en los
demás solo cuando el cursor pasa por encima.

- **El botón no integra nada**: manda un mensaje al agente que está dentro de ese worktree.
- **La etiqueta dice el destino** deducido del historial de la propia rama: hacer merge en esa rama,
  abrir un pull request hacia ella, o solo avisar que terminó.
- **El menú del botón** cambia el modo. La elección vale para ese destino y queda guardada.
- **Reanudar**, en los frentes parados o vacíos sin nadie dentro: abre un agente nuevo y lo manda
  entrar en ese worktree. El botón no aparece cuando el frente ya tiene agente.

En **Ajustes → Interfaz**:

- **Cómo entregar un frente terminado**: elige el modo predeterminado de todos los destinos de todos
  los proyectos. Deducir de cada destino mira cómo entró el trabajo en esa rama antes y sugiere lo
  mismo. La elección hecha en el menú de la barra manda por encima, y solo en ese destino.
- **Editar el mensaje…**: reescribe el texto que envía el botón. Los tres marcadores se convierten en
  el nombre de la rama, el destino y el verbo del modo elegido, y sin el marcador de la acción el
  mensaje no dice qué hacer.

## Cuando varios terminan a la vez

Un agente que acaba de integrar puede pasar el turno al siguiente de la fila, y el siguiente recibe
en su panel el aviso de que llegó su turno. Esto solo alcanza a agentes vivos de este canvas: quien
fue despedido o está en otro canvas no es despertado.

## Configurado en otra pantalla

- Las áreas de trabajo que son las secciones de la barra: [áreas de trabajo](areas-de-trabalho).
- El estado de cada agente: [saber qué están haciendo](saber-o-que-fazem).
- El repositorio en el canvas: [el agente y el repositorio](o-agente-e-o-git).
