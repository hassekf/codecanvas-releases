---
slug: varios-canvases
titulo: Varios canvases
resumo: Cada canvas es un proyecto con su carpeta: crear, cambiar sin interrumpir a nadie, cerrar, y la pantalla inicial.
area: canvas
nivel: basico
---

Un canvas es un proyecto: un nombre y una carpeta. Todo agente creado en él nace en esa carpeta,
descrita en [elegir el proyecto](escolher-o-projeto).

## Crear

El selector de proyecto está a la izquierda de la barra de comandos y muestra el nombre del canvas
abierto. Haz clic en él y elige **Nuevo canvas…**.

- **La carpeta es obligatoria**: el botón **Crear** queda no disponible mientras no se elija una.
- **El nombre es opcional**: en blanco, la app usa el nombre de la carpeta.
- Al crear aparecen cinco secciones: Proyecto, Agentes, MCP, Navegador y Apariencia. Skills, Anuncios
  e Integraciones solo existen una vez creado el proyecto. Ver
  [ajustes del proyecto](ajustes-projeto).
- **Por voz**, *"crea un proyecto nuevo"* abre esta misma ventana, y la carpeta se elige en ella.

## Cambiar

- **El selector de proyecto**, en la barra de comandos.
- **Dos toques rápidos en ←** retrocede un proyecto, **dos en →** avanza uno, dando la vuelta al
  final de la lista. El atajo no se dispara con ningún modificador pulsado, ni mientras escribes en
  un agente o en un campo de texto.
- **⌘1 a ⌘9**, por la posición del proyecto en la pantalla inicial. Las teclas se cambian en
  **Ajustes → Atajos**, como está en [mover y hacer zoom](mover-e-dar-zoom).
- **Por voz**: *"cambia al proyecto platform"*.

Cambiar no interrumpe nada. Los agentes del proyecto que salió de la vista siguen trabajando, y los
navegadores quedan como estaban.

## Quién te espera en otro proyecto

El selector muestra un contador cuando **otro** canvas tiene agentes esperándote. Su menú lo detalla
proyecto por proyecto: cuántos están esperando, cuántos están trabajando y cuántos avisos llegaron
allí mientras estabas fuera. El proyecto abierto no trae esa cuenta de avisos, porque se pone a cero
cuando entras en él.

## Cerrar un canvas

La opción está al final del menú del selector y solo aparece con más de un canvas. Pide
confirmación, y lo que hace es esto: cierra los agentes de ese proyecto y saca el canvas de la
lista. La carpeta del proyecto y el código no se tocan, y no hay forma de deshacerlo.

Cambiar de canvas no cierra a nadie. Volver a la pantalla inicial tampoco.

## La pantalla inicial

La app abre en ella, y no en el último proyecto. Cada proyecto es una tarjeta con el paisaje y el
color de su tema, la ruta de la carpeta, cuántos agentes están trabajando ahí ahora (o el tamaño del
elenco, si no hay ninguno) y hace cuánto estuviste en él. El último proyecto abierto recibe la marca
**DÓNDE TE QUEDASTE** cuando hay más de uno.

- **PROYECTOS RECIENTES**, debajo de la cuadrícula: los cinco últimos que abriste, por orden de uso.
  Aparece a partir de dos proyectos.
- **Editar un proyecto**: el **⋯** de la esquina de la tarjeta, o el clic derecho en ella.
- **Volver a la pantalla inicial** desde dentro de un canvas: **Pantalla inicial**, arriba del todo
  en el menú del selector de proyecto.

### El orden de las tarjetas

Arrastra una tarjeta sobre otra para reordenarlas, con el contorno encendido diciendo dónde va a
caer. El orden queda guardado, y es el que da la tecla: la posición 1 responde a ⌘1, y así hasta la
novena. El número aparece en la esquina de la tarjeta y al lado de la fila en PROYECTOS RECIENTES.
Del décimo proyecto en adelante no hay tecla.

Desde dentro de otro canvas la tecla cambia de proyecto y el aviso dice el nombre del que se abrió.
Es el mismo orden que recorren los dos toques en las flechas.

## Lo que es de cada canvas

El tema, la fuente de la interfaz, el fondo, la página en la que abre un navegador nuevo, la cuenta
en la que nacen los agentes, las skills, los servidores MCP, los anuncios, las integraciones y las
áreas de trabajo son de cada proyecto. El Jira conectado en uno no aparece en el otro.

Lo que vale para todos los proyectos está en **⌘,**, los ajustes de la app. Ver
[ajustes del proyecto](ajustes-projeto) y [la cara del proyecto](aparencia).
