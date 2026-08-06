---
slug: painel-galeria
titulo: La galería de imágenes
resumo: Las imágenes de este proyecto guardadas en disco: devolverlas al lienzo, eliminarlas de verdad, y el prompt que generó cada una.
area: paineis
nivel: basico
---

Se abre con `⌘K` (escribe "galeria" o "imagens"). Hay una por proyecto.

## Qué guarda

Toda imagen que entró en el lienzo de este proyecto, pegada, arrastrada o generada. Quitar una
imagen del lienzo no borra el archivo: sigue aquí, y la eliminación definitiva ocurre **solo** en
este panel.

En la miniatura y en la leyenda:

- **Generada**: la leyenda es el prompt que creó la imagen, y un distintivo la marca en la
  miniatura.
- **Pegada**: la leyenda dice solo eso, porque no hay prompt guardado.
- Un segundo distintivo marca las imágenes que están puestas en el lienzo en este momento.

## Los gestos de la cuadrícula

- **Clic en una miniatura**: marca y desmarca. Hacer clic en varias marca varias.
- **Arrastrar desde un hueco**: dibuja un lazo y marca todo lo que toca, entre las miniaturas
  visibles. Un clic en el hueco limpia la selección.
- **Arrastrar una miniatura**: lleva la imagen al lienzo. Si pertenece a una selección de varias, el
  arrastre lleva todas las marcadas, cada una desplazada de la anterior.
- **El `+` al pasar el ratón**: devuelve la imagen al lienzo sin arrastrar.

## El menú de cada imagen

- **Añadir al lienzo**: devuelve la imagen al lienzo.
- **Enviar a un contacto**: manda la imagen por [recados](painel-recados). El prompt que la generó
  se convierte en el asunto.
- **Copiar el prompt**: copia el prompt al portapapeles. Solo existe en imagen generada.
- **Eliminar de la galería**: borra el archivo, con confirmación.

## La cabecera

- **El número junto al título**: cuántas imágenes tiene el proyecto.
- **Eliminar (n)**: elimina las marcadas, con confirmación. Aparece cuando hay algo marcado.
- **Limpiar selección**: desmarca todo sin borrar nada.
- **Seleccionar todo**, **Actualizar** y **Vaciar toda la galería**, en el menú al lado: el segundo
  relee la carpeta del disco; el tercero elimina todas las imágenes del proyecto, con confirmación.

## Eliminar también la quita del lienzo

La confirmación cambia cuando alguna de las imágenes a eliminar está puesta en el lienzo: pregunta
**¿Eliminar también del lienzo?** y nombra las áreas de trabajo donde está la imagen. Eliminar de la
galería quita la imagen del lienzo también, y no se puede deshacer.

## Cómo se genera una imagen

Pídesela a la asistente por voz, o a un agente por escrito. Puedes decir cuántas imágenes quieres
(una es lo predeterminado), la orientación (cuadrado es lo predeterminado, y hay horizontal y
vertical) y la calidad de ese pedido.

La generación tarda decenas de segundos: la app responde antes de terminar, pone cada imagen en el
lienzo cuando queda lista y avisa al final. Pedida a un agente, la imagen nace cerca de su panel;
pedida por voz, nace en espacio libre en el centro de la vista.

El prompt y el modelo quedan guardados con el archivo. Es lo que muestra la leyenda y lo que
entrega **Copiar el prompt**.

Esto no es el fondo de pantalla del lienzo, que tiene comandos propios en
[apariencia](aparencia).

### El modelo y la calidad predeterminados

En **Configuración → Conversación**.

- **Modelo de imagen**: el modelo que dibuja. La lista se consulta a OpenAI, y **Actualizar** la
  relee.
- **Calidad de imagen predeterminada**: **Económica**, **Predeterminado** o **Alta**. Vale para los
  pedidos que no piden otra calidad.

Los dos dependen de que tu clave de OpenAI esté registrada, en la misma pantalla. Ver
[configurar la voz](configurar-a-voz) y [cuánto cuesta](quanto-custa).

## Las imágenes sueltas en el lienzo

Poner una imagen en el lienzo, moverla, cambiar su capa y borrarla están en
[imágenes en el lienzo](imagens-no-canvas). Esta página trata de dónde quedan guardadas.
