---
slug: o-agente-desenha-e-gera
titulo: El agente diseña y genera imágenes
resumo: Pedir pantallas en la superficie de diseño, señalar qué cambiar, generar imágenes en el lienzo y usar las referencias que pegaste.
area: agentes-fazem
nivel: avancado
---

## Qué pedir

- *"Diseña tres variaciones de la pantalla de inicio de sesión: una clásica, una con foto de fondo,
  una minimalista."*
- *"Haz ese botón más grande y con más aire debajo."*
- *"Diseña el flujo de registro, cuatro pantallas."*
- *"Trae una fuente mejor para los títulos."*
- *"Genera una mascota de zorro, plana, fondo blanco."*
- *"Mira las referencias que pegué en el lienzo y sigue ese clima."*

Qué es la superficie de diseño y qué guarda está en [el panel de diseño](painel-design).

## Diseñar

El agente lee el archivo de diseño, lo edita y fotografía el resultado. Ves cada cambio aparecer en
el panel mientras ocurre.

- Crea y modifica artboards, marcos, rectángulos, elipses, textos, trazados, imágenes e iconos, con
  disposición, relleno, contorno, esquina redondeada, sombra y desenfoque.
- Define los **tokens** del archivo, el vocabulario de colores y medidas con el que pintan todos los
  agentes.
- **Una pantalla nueva, una variación o la versión móvil de algo entran como artboard en el archivo
  abierto.** Un paquete nuevo solo nace cuando cambia el asunto o cuando lo pides por separado.
- **Tú no dibujas a mano.** No hay tiradores, ni inspector, ni texto editable en el panel. Tus gestos
  sobre el diseño son mover pantallas y señalar.

## Señalar

Haz clic en un elemento del diseño, o lazea una región, y la petición pasa a tener referente.

- La selección viaja con el mensaje: un recorte en imagen de lo que señalaste, más los
  identificadores y las medidas de ese fragmento.
- El agente que recibe el señalamiento se elige en el propio panel de diseño, y la elección queda
  guardada entre una petición y la siguiente.
- **Siete palabras llevan instrucción de dirección cuando aparecen en lo que escribes**: `mais
  ousado`, `mais quieto`, `polir`, `mais denso`, `mais leve`, `variar` y `alinhar`. Valen para la
  región señalada.

## Varias pantallas a la vez

Una petición con muchas pantallas o muchas variaciones se convierte en un agente por pantalla, cada
uno limitado a su propio artboard, trabajando a la vez. Quien reparte es el agente que recibió la
petición, por la misma vía de [el agente llama colegas](o-agente-chama-colegas).

## La dirección del archivo

Todo diseño tiene una dirección escrita: el estilo, el resumen del producto, el tono, lo memorable de
la pantalla, la paleta y el par de fuentes. Se rellena cuando nace el diseño, y la reabres y editas
después.

- Un agente no cambia el estilo, la paleta ni las fuentes del archivo sin que se lo pidas.
- Un archivo sin dirección no recibe el primer elemento: se manda al agente escribirla antes.

## Tipografía

- **Medir**: el agente mide un texto con la fuente real del archivo antes de insertarlo, y recibe
  ancho y alto en píxeles. Para un párrafo, pasa el ancho máximo y recibe el alto con los saltos
  reales. La medida es del texto puro, sin el relleno interno de la caja.
- **Traer una familia de Google Fonts** al paquete, con los pesos que vaya a usar. La descarga ocurre
  en segundo plano y los textos cambian de fuente cuando termina. A partir de ahí la fuente viaja con
  el archivo y funciona sin red.

## Generar imágenes

La imagen nace en el lienzo, en espacio libre al lado del panel de quien la pidió.

- El agente elige la cantidad y la orientación: horizontal, vertical o cuadrada.
- El modelo y la calidad vienen de tu Configuración. Puede pedir otra calidad solo en esa llamada,
  entre baja, media y alta.
- El tope del modelo vence a la cantidad pedida: algunos generan una imagen por vez.
- Toda imagen generada queda en la [galería](painel-galeria), con la petición que la creó.
- Esto no es el fondo de pantalla. El fondo se cambia en [apariencia](aparencia).
- Generar imágenes usa tu clave de OpenAI, la misma de la voz. Sin ella, el agente recibe el aviso de
  que falta la clave.

## Las referencias que pegaste

Las imágenes que pegas o arrastras al lienzo quedan disponibles para los agentes. Un agente lista
esas imágenes y abre cada una por su ruta, y ve el contenido de ellas.

Sirve para capturas de error, fotos de pantalla y bocetos de papel fotografiados, sin que describas
en palabras lo que hay en la figura.
