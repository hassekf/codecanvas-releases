---
slug: design-no-canvas
titulo: Diseño en el lienzo
resumo: La superficie donde los agentes dibujan pantallas y tú diriges señalando, con el archivo versionado en el proyecto.
area: design
nivel: basico
---

CanvasCode tiene una superficie de diseño propia. **Los agentes dibujan, y tú diriges**: haces clic
en un elemento o encierras una región con el lazo y pides desde ahí. Cada agente que está dibujando
aparece con un cursor propio en la pantalla.

Tú no editas a mano. No hay manijas, ni inspector, ni texto editable en el panel, y tus gestos sobre
un diseño son dos: mover artboards y señalar.

## El archivo

Un diseño es una carpeta con extensión `.design`, que el Finder muestra como si fuera un archivo.
Dentro de ella están el documento y las imágenes e iconos que usa.

- **Suele vivir en el repositorio del proyecto**, versionado con el código. El dibujo entra en el
  historial, viaja a quien clone el proyecto y cualquier agente puede leerlo como especificación.
- **Un diseño abierto no es un panel**: se abre en el plano del lienzo, con los artboards sueltos
  ahí.
- **Cada pantalla, variación o versión móvil es un artboard** dentro del mismo archivo. Un archivo
  nuevo solo nace cuando cambia el asunto.

## Qué se puede pedir

- **Pantallas y variaciones**: *"dibuja tres variaciones de la pantalla de login: una clásica, una
  con foto de fondo, una minimalista"*. Un pedido con muchas pantallas se convierte en un agente por
  pantalla, dibujando al mismo tiempo.
- **Ajustes señalados**: selecciona un botón y pide *"hazlo más grande y con más aire debajo"*.
- **Flujos enteros**: *"dibuja el flujo de registro, cuatro pantallas"*.
- **Tipografía de verdad**: el agente trae una familia de Google Fonts al paquete, con los pesos que
  use. De ahí en adelante la fuente viaja con el archivo y funciona sin internet.
- **Iconos**: usa un catálogo de unos dos mil iconos, y lo que use queda grabado dentro del paquete.
- **Seguir referencias**: las imágenes que pegaste en el lienzo quedan disponibles para él. Ver
  [imágenes en el lienzo](imagens-no-canvas).

Lo que el agente hace mientras dibuja, y lo que mide y comprueba antes de entregar, está en [el
agente diseña y genera](o-agente-desenha-e-gera).

## Los tokens

El archivo guarda su propio vocabulario de colores y medidas, y es con él que pintan todos los
agentes. Cambiar un token cambia todo lo que lo usa, en todos los artboards, de una vez. Un agente
que necesita un color nuevo declara un token en vez de escribir el color suelto.

## La dirección

Todo diseño tiene una dirección escrita dentro del archivo: el pedido, el estilo, el tono, la paleta,
el par tipográfico y las reglas que el agente tiene que respetar. Es ella la que hace que dos agentes
dibujen la misma cosa en vez de dos productos diferentes. Ver [la dirección del
diseño](design-direcao).

## Qué no es

- **No es un editor tipo Figma.** Es un recorte de producto: quienes dibujan son los agentes.
- **No exporta a imagen ni a código** hoy.
- **No es el panel de imágenes.** Una imagen generada es otra cosa, y vive en la
  [galería](painel-galeria).

Para programar a partir del dibujo, un agente lee el propio archivo del diseño: es la
especificación, y no necesita exportación.

## Por dónde empezar

1. `⌘⇧D`, o el pincel del pie, abre el navegador de diseño.
2. **Nuevo diseño** pide la dirección y crea el archivo.
3. Elige quién dibuja, y pide la primera pantalla.

La pantalla y los gestos están en [la superficie de diseño](painel-design).
