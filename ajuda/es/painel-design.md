---
slug: painel-design
titulo: La superficie de diseño
resumo: Dónde viven los artboards en el lienzo, cómo se navega por ellos, y cómo señalar un trecho se vuelve un pedido a un agente.
area: design
nivel: avancado
---

Un archivo de diseño es una carpeta con extensión `.design`, que suele vivir en el repositorio del
proyecto. Se abre **en el plano del lienzo**: los artboards quedan sueltos ahí, sin marco de panel.

- **`⌘K` y design**, **artboard**, **mockup**, **prototipo**, **interfaz**, **layout**, **figma**,
  **wireframe** o **dibujo**: abre el primer `.design` de la raíz del proyecto. Si no hay ninguno, la
  app abre antes la pantalla de dirección y crea uno.
- **`⌘⇧D`, o el pincel del pie**: abre el navegador de diseño.

Tú no editas a mano: no hay manijas ni inspector. Tus gestos sobre un diseño son mover artboards y
señalar. Quienes dibujan son los agentes, cada uno con el cursor visible en la pantalla.

## El navegador de diseño

- **En el lienzo**: los diseños en escena. Al hacer clic en el nombre se pliega y despliega su lista
  de artboards; el número al lado del nombre cuenta los artboards.
- **Una línea de artboard**: lleva la cámara hasta él. La línea del artboard que está en la selección
  viva aparece destacada.
- **El lápiz**, en la línea del diseño: reabre la dirección de ese archivo, ya rellenada.
- **La flecha**, en la línea del diseño: lleva la cámara hasta el diseño entero.
- **Cerrar diseño**, en el menú contextual de la línea: saca el diseño de la escena sin borrar el
  archivo.
- **Quitar artboard** y **Enviar a un contacto**, en el menú contextual de un artboard: borra el
  artboard del archivo, o manda el documento a un contacto, con el nombre del artboard como asunto.
- **En el proyecto**: los paquetes `.design` de la raíz del workspace que todavía no están en escena.
  **Abrir** trae uno de ellos al lienzo.
- **Nuevo diseño**: abre la pantalla de dirección y crea un archivo.

Pulsar `⌘⇧D` de nuevo cierra el navegador.

## La dirección

La dirección queda guardada dentro del archivo y vale para cualquier agente que dibuje ahí después.
La pantalla pide:

- **Nombre**: el nombre del archivo. Solo al crearlo.
- **El pedido**: el brief. Es el único campo que la pantalla trata como necesario.
- **Dirección**: uno de los estilos ofrecidos, o **El agente decide**.
- **Varianza estructural** y **Densidad**: dos deslizadores, de seguro a experimental y de esparcido
  a denso.
- **Tema** (**Claro**, **Oscuro**, **Ambos**) y **Objetivo** (**Desktop**, **Móvil**, **Ambos**).
- **Color semilla**: un color de partida, o **Auto**.
- **Tipografía**: el par tipográfico. Vacío, lo elige el agente.
- **Reglas avanzadas**: cuatro reglas que el agente recibe junto con lo demás, cada una con su
  interruptor: la ban-list anti-slop, el uso obligatorio de los tokens del archivo, la auditoría
  visual antes de entregar, y la exigencia de que las variaciones cambien de esqueleto.
- **Quién diseña**: **Nadie por ahora**, **Un agente nuevo**, o un agente abierto en el lienzo. El
  botón del pie cambia según la elección.

Lo que dejes en blanco lo elige el agente, lo declara y lo graba en el archivo.

## Señalar

Haz clic en un elemento o encierra una región con el lazo: una caja nace pegada a la selección.

- **Los verbos** (*mais ousado*, *mais quieto*, *polir*, *mais denso*, *mais leve*, *variar*,
  *alinhar*): cada toque agrega la palabra a tu texto. Reconocida al enviar, lleva junto una
  instrucción de dirección para el agente.
- **El campo de pedido**: `Enter` envía.
- **El nombre a la derecha del campo**: elige el agente que lo recibe. La lista pone delante los
  agentes de la misma área de trabajo y los despiertos. La elección queda guardada y no se pierde al
  cambiar de selección ni al enviar.

El agente recibe tu texto, la descripción de lo que seleccionaste, un recorte en imagen del trecho,
un manifiesto con los ids y la ruta del archivo. En un diseño todavía vacío, la caja aparece igual y
al agente se le avisa de que no hay ningún artboard.

La selección sigue viva después del envío: cualquier agente que lea el diseño encuentra ahí el
referente de *"ese botón"*.

## Arrastrar un artboard hacia afuera

Sacar un artboard de la superficie lo convierte en una tarjeta que sigue al cursor. Soltada sobre un
panel de agente, él recibe la cita de ese artboard (el recorte, los ids y el archivo). Soltada en el
vacío, no pasa nada y el documento no cambia.

## El zoom

El zoom y el arrastre del lienzo son los del diseño: no hay una cámara dentro de otra, y la
superficie no se desplaza por su cuenta.

## Cuando el archivo tiene un problema

- **Archivo que la app no pudo leer**: el paquete queda bloqueado. Las herramientas de los agentes
  responden con la lista de problemas y **no se graba nada**. Corregido el archivo, se desbloquea
  solo.
- **Archivo cambiado por fuera** (un agente editando el `design.json` directo, un `git checkout`): la
  app lo recarga. Si hay conflicto con lo que estaba en memoria, gana el disco y la app lo avisa.

## Qué hacen los agentes aquí

Leen el documento y tu selección, aplican operaciones, fotografían el resultado, miden un texto antes
de insertarlo y traen una fuente de Google Fonts al paquete. Está en
[el agente diseña y genera](o-agente-desenha-e-gera).

Exportar el diseño a imagen o a código no existe hoy.
