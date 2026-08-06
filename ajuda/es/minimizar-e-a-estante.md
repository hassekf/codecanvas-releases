---
slug: minimizar-e-a-estante
titulo: Minimizar y el estante
resumo: Guardar un panel sin cerrarlo, y la lista de todo lo que está abierto en este proyecto.
area: canvas
nivel: basico
---

## Minimizar

El botón **−** en la cabecera de cualquier panel, o el menú del botón derecho → **Minimizar**.

El panel sale de la pantalla y el contenido sigue vivo: el agente sigue trabajando y sigue cambiando
de estado, y la página del navegador sigue cargada, con el historial y lo que hubieras rellenado. El
aviso que aparece trae **Traer de vuelta**, que lo restaura y lleva la cámara hasta él.

Dos excepciones:

- **Los medios** se convierten en una cápsula al lado de la barra de comandos, con las barritas de
  sonido, el play y la pausa. El sonido no se detiene. Ver [el panel de medios](painel-midia).
- **Un agente que trabaja en un paso de una Iniciativa** no tiene el botón de minimizar. En su lugar
  hay uno de ocultar, que devuelve el panel fuera de tu vista sin cerrar nada. Ver
  [el panel de Iniciativas](painel-iniciativas).

## Abrir el estante

- **⌘⇧E**, que también lo cierra.
- **El botón del estante**, en la barra de comandos. Se destaca cuando un agente guardado te está
  esperando, está trabajando o se ha caído.
- **El contador de paneles**, en la misma barra. Muestra cuántos paneles están abiertos en la
  cuadrícula automática, y el zoom de la cámara en el lienzo libre.

Los dos se pueden ocultar en **Ajustes → Interfaz**, en el bloque **Elementos de la barra de
comandos**. Oculto, el elemento pasa detrás de la flecha del final de la barra.

## Lo que muestra la lista

El número de arriba es el total de paneles de este canvas, sumando todas las áreas.

- **El selector de área**, justo debajo del título: elige de qué [área de trabajo](areas-de-trabalho)
  es la lista. Es la misma navegación que las pestañas del lienzo: elegir aquí cambia de pestaña, y
  cambiar de pestaña cambia aquí. Con una sola área, se convierte en una etiqueta.
- **El filtro por tipo**: **Todo**, **Agentes**, **Navegadores**, **Documentos**, **Diseños** y
  **Otros**. Corta la lista dentro del área elegida, y solo aparece cuando esa área tiene más de un
  tipo.
- **Cada fila** trae el icono, el nombre y, cuando un agente abrió ese panel, de quién es. Un agente
  que no está ocioso recibe un punto de estado al lado del nombre.
- Los paneles guardados bajan al final de la lista y siguen en su área.

## Ir hasta él, o traerlo hasta ti

- **Hacer clic en la fila**: lleva la cámara hasta el panel, que se queda donde está. Si estaba
  guardado, se restaura en su sitio y la cámara va con él.
- **El botón de traer**, a la derecha: trae el panel al centro de tu pantalla y, si estaba en otra
  área, al área abierta. Solo aparece donde la posición es del panel: en el lienzo libre, o en un
  panel suelto de la cuadrícula. En la cuadrícula automática la disposición reescribiría la posición
  al instante siguiente.
- **El botón de al lado**: minimiza el panel, o lo saca del estante y lo devuelve a su sitio.

## Guardar y mostrar en lote

Los dos botones del pie actúan sobre **lo que está listado arriba**: el área elegida en el selector,
cortada por el filtro.

- **Mostrar**: saca del estante todos los guardados de esa lista, cada uno en su sitio. La cámara no
  se mueve.
- **Minimizar**: guarda todos los que están en pantalla. Solo aparece a partir de dos. El aviso trae
  **Deshacer**, que devuelve exactamente esos, y no todos los que estaban guardados.
