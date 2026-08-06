---
slug: design-direcao
titulo: La dirección del diseño
resumo: El briefing grabado dentro del archivo de diseño, que todo agente que dibuje ahí recibe antes del primer píxel.
area: design
nivel: basico
---

La dirección es el briefing del archivo. Queda guardada dentro del `.design`, viaja con él y vale
para **cualquier** agente que dibuje ahí después, incluidos los que abras mañana.

Un archivo sin dirección no recibe el primer elemento: al agente se le manda escribirla antes de
dibujar.

## Dónde se escribe

- **Al crear un diseño**: la pantalla de dirección se abre antes de que el archivo exista. **Nuevo
  diseño**, en el navegador de diseño (`⌘⇧D`).
- **Después**: el lápiz en la línea de ese diseño, en el navegador, reabre la pantalla rellenada.

## Qué pide

- **Nombre**: el nombre del archivo. Solo al crearlo.
- **El pedido**: el briefing, en texto libre. Es el único campo que la pantalla trata como necesario.
- **Dirección**: uno de los estilos ofrecidos, o **El agente decide**.
- **Varianza estructural** y **Densidad**: dos deslizadores, de seguro a experimental y de esparcido
  a denso.
- **Tema**: **Claro**, **Oscuro** o **Ambos**.
- **Objetivo**: **Desktop**, **Móvil** o **Ambos**.
- **Color semilla**: un color de partida, o **Auto**.
- **Tipografía**: el par tipográfico. Vacío, lo elige el agente.
- **Quién diseña**: **Nadie por ahora**, **Un agente nuevo**, o un agente ya abierto en el lienzo.

**Lo que dejes en blanco, el agente lo elige, lo declara y lo graba en el archivo.** La dirección deja
de tener huecos después del primer trabajo, y el agente siguiente encuentra la decisión tomada en vez
de inventar otra.

## Las reglas avanzadas

Cuatro interruptores que entran junto con la dirección:

- **La ban-list**: la lista de lo que no puede aparecer en el dibujo.
- **Usar los tokens del archivo**: obliga al agente a pintar con el vocabulario de colores y medidas
  del documento, en vez de escribir valores sueltos.
- **Auditoría visual antes de entregar**: el agente fotografía y comprueba su propio resultado antes
  de decir que terminó.
- **Una variación cambia de esqueleto**: una variación tiene que cambiar la estructura, y no solo el
  color.

## Qué gobierna la dirección

- **Estilo, paleta y fuentes no cambian sin que tú lo pidas.** Un agente que cree que quedaría mejor
  de otro modo propone, no cambia.
- **Los verbos del señalamiento** (*mais ousado*, *mais quieto*, *polir*, *mais denso*, *mais leve*,
  *variar*, *alinhar*) llevan una instrucción de dirección junto con tu pedido, y valen para la región
  que señalaste. Ver [la superficie de diseño](painel-design).
- **Cada agente recibe solo el capítulo que ese archivo pide**, y no la doctrina entera.

## Cambiar la dirección después

Reabrir y guardar vale para lo que se dibuje de ahí en adelante. Lo que ya está en el archivo sigue
como está: cambiar la dirección no repinta ningún artboard. Para alinear lo que ya existe, pídelo.
