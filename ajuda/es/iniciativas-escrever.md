---
slug: iniciativas-escrever
titulo: Escribir una Iniciativa
resumo: Los dos caminos para crear el archivo del proceso conversando con un agente, y cómo cambiarlo después.
area: iniciativas
nivel: avancado
---

No rellenas ningún formulario: **quien escribe el archivo es un agente, conversando contigo**. El
panel de Iniciativas abre la conversación y le dice al agente dónde guardarlo.

## Los dos caminos

Los dos están en la pantalla del panel cuando el proyecto todavía no tiene ninguna Iniciativa, y en
**Nueva iniciativa** después de eso. En los dos eliges qué agente lo recibe, y la conversación ocurre
en su panel.

### Escribirla desde cero, conversando

El agente **no lee el proyecto y no propone nada** al abrirse. Responde una línea diciendo que está
listo y espera a que le cuentes qué proceso quieres describir.

A partir de ahí pregunta lo que falte, en vez de rellenarlo por su cuenta: las etapas en orden, qué
produce cada una, qué bloquea, y dónde aprueba alguien. Solo guarda el archivo cuando el proceso está
cerrado contigo.

Es el camino para un proceso que existe en tu cabeza, o que todavía va a existir.

### Leer el proyecto y proponer

El agente recibe junto lo que el panel ya encontró en el repositorio sin leer nada: los comandos, los
scripts de validación y las ejecuciones antiguas. Lee esos archivos, monta la cadena a partir de lo
que **está escrito**, pregunta lo que falte en vez de inventar, guarda y entonces te cuenta en cinco
líneas lo que entendió, para que compruebes si coincide con lo que el equipo hace de verdad.

Es el camino para un proceso que ya está en el proyecto, repartido en scripts.

## Qué describe el archivo

El agente escribe esto; vale la pena saber qué te va a preguntar:

- **Cómo empieza una ejecución**: qué exige la Iniciativa para empezar, una fuente, un texto, una
  lista de preguntas, la salida de otra ejecución, o nada.
- **Los pasos, en orden**: el nombre de cada uno, qué entra, qué sale, y quién lo ejecuta (un comando,
  o un agente con su instrucción).
- **La puerta de un paso**: el comando que prueba que el resultado sirve. Sin puerta, el paso pasa con
  la palabra del agente.
- **La firma**: el momento en que la ejecución se detiene y te espera, con lo que muestra y la
  etiqueta del botón de aprobar.
- **La revisión**: un paso cuya salida es un veredicto, que aprueba, rechaza o bloquea el trabajo.
- **El tope de vueltas** de cada ruta de corrección.

## Cambiarla después

En la pantalla de la Iniciativa:

- **Editar con un agente**: manda el archivo y lo que quieres cambiar al agente que elijas.
- **Ver los orígenes**: los archivos del proyecto de donde salió la Iniciativa, cada uno marcado como
  **apunta** (la ejecución lee la versión de ahora) o **copia** (la ejecución usa la versión guardada
  en la Iniciativa).
- **Ver qué cambió**: aparece cuando un archivo de origen cambió después de que la Iniciativa fue
  escrita. **Releer con el agente** le manda el archivo, lo que cambió y la Iniciativa que salió de
  ahí; lo lee y responde qué quedó desactualizado, sin tocar nada.

**Editar la Iniciativa con una ejecución en curso cambia esa ejecución en marcha**, y la pantalla de
la ejecución avisa cuando eso pasó.

## Cuando el archivo tiene error

Un archivo que la app no consiguió leer aparece igualmente en la lista, marcado, y su pantalla
enumera cada rechazo con el campo y el motivo. El menú ofrece **Ver los problemas**, **Pedirle a un
agente que lo arregle** y **Abrir el archivo**.

## Por dónde seguir

- El concepto y el vocabulario: [qué es una Iniciativa](iniciativas-o-que-e).
- Ejecutar y seguir: [el panel de Iniciativas](painel-iniciativas).
