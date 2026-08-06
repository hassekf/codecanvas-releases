---
slug: painel-modulos
titulo: El panel de un módulo
resumo: Cómo abrir un panel escrito por ti, qué hace su barra, y los dos interruptores de cada módulo.
area: modulos
nivel: avancado
---

Un módulo es un panel escrito por ti (o por un agente tuyo) e instalado en una carpeta de tu Mac.
Para escribir uno, mira [módulos](modulos).

Ábrelo con `⌘K` y el nombre del módulo, o las palabras de búsqueda que declaró su manifiesto. Por
voz, el módulo se abre por el nombre del manifiesto.

Por defecto es un panel por lienzo: pedir el mismo módulo de nuevo selecciona el panel que ya existe.
Un módulo puede declarar que acepta varios.

El módulo está disponible en todos los proyectos. Cada
apertura crea un panel de ese lienzo, y la página sabe en qué proyecto está: el mismo módulo puede
mostrar cosas distintas en cada uno.

## La barra del panel

- **La línea de la izquierda**: la descripción del manifiesto.
- **Recargar el módulo**: recarga la página.
- **Mostrar la carpeta en Finder**: abre la carpeta del módulo.

Un módulo puede declarar que vive fuera de la cuadrícula. En ese caso la cabecera, el borde y esta
barra desaparecen mientras el panel está suelto, y el contenido llena el panel entero; un clic
revela los controles de nuevo, y devolverlo a la cuadrícula trae el marco.

Un módulo también puede declarar un intervalo de recarga (mínimo cinco segundos), y entonces la
página se recarga sola.

## Mientras escribes el módulo

La app vigila la carpeta: guardar un archivo recarga los paneles de ese módulo, sin reiniciar nada y
sin reabrir el panel. Los paneles de otros módulos no se tocan.

El panel también habla cuando algo está mal, en vez de quedarse en blanco:

- **Este módulo tiene un problema**: el manifiesto o la carpeta no pasaron la validación. El texto
  dice qué, y el botón muestra la carpeta en Finder.
- **Este módulo ya no existe**: la carpeta desapareció del disco. Si vuelve, el panel vuelve con
  ella.
- **Este módulo está desactivado**: el módulo está entero, pero apagado en Configuración.

Un error de JavaScript de la página no tumba la app: se queda en la consola de esa página, y los
agentes leen esa consola.

## Configuración → Módulos

La pantalla lista los módulos válidos y los que no pasaron la validación, estos con el motivo escrito
y un botón **Mostrar**.

- **El interruptor de cada módulo**: apagado, el módulo desaparece de la búsqueda, de la voz y del
  alcance de los agentes. Un panel suyo que esté abierto dice que el módulo está desactivado, en vez
  de desaparecer de tu vista.
- **Herramientas para Nina**: solo aparece en un módulo activo y con acciones. Apagado, la asistente
  vuelve a solo abrir y cerrar el panel, y las acciones salen de su vocabulario en la próxima
  conversación.
- **Mostrar la carpeta de módulos en Finder**, al pie: abre la carpeta donde viven todos.

Un módulo nuevo nace activo y con las acciones disponibles.
