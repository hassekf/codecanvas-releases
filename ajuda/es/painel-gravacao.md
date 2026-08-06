---
slug: painel-gravacao
titulo: Grabar la pantalla
resumo: Grabar la ventana de CanvasCode con el audio de la app y el micrófono: formato, calidad, y qué hacer con el archivo después.
area: paineis
nivel: basico
---

Se abre con `⌘K` (escribe "gravação" o "gravar").

## Qué entra en la grabación

La **ventana de CanvasCode**, el audio que produce la app y tu micrófono. Nada que pase por encima
de la ventana aparece en el vídeo, y no entra el sonido de ninguna otra app. La resolución de salida
viene del tamaño real de la ventana en píxeles, Retina incluido.

macOS pide el permiso de **Grabación de Pantalla** la primera vez, y la grabación no empieza sin él:
el panel muestra el aviso con la ruta para autorizarlo. Ver
[los permisos que pide macOS](permissoes-do-mac).

## Los controles

- **El botón central**: empieza a grabar, y retoma una grabación pausada. Mientras graba, queda
  desactivado.
- **Pausar**: interrumpe sin terminar.
- **Detener**: termina y guarda el archivo.
- **El reloj** cuenta el tiempo grabado, y la línea de abajo dice el estado: **Listo para grabar**,
  **Grabando** o **Pausado**.

No hay límite de tiempo.

**La pausa no recorta ese tramo.** El tiempo pausado se convierte en un fotograma congelado con la
duración de la pausa, en el vídeo final.

## Formato de la ventana

Cuatro botones que redimensionan la **ventana de la app** antes de grabar: **Horizontal · 4K**
(3840×2160), **Horizontal · 1080p** (1920×1080), **Vertical · Story** (1080×1920) y **Cuadrado**
(1080×1080).

## Calidad

Los controles de esta sección solo funcionan con la grabación detenida, y el panel lo dice cuando
está en curso.

- **Máxima · editar**: sin objetivo de tasa de bits. El archivo es grande, y sirve para quien va a
  editar y volver a comprimir después.
- **Equilibrada**: lo predeterminado. La tasa de bits acompaña el tamaño de la ventana.
- **Compacta · chat**: tasa menor, y la captura sale en 1×, sin Retina.
- **30 fps** y **60 fps**: fotogramas por segundo. 60 fps produce un archivo mayor.
- **H.264 · compatible** y **HEVC · compacto**: el códec. HEVC genera un archivo menor con el mismo
  resultado visual; H.264 se reproduce en más sitios.
- **Audio en una pista · compartir** y **Pistas separadas · editar**: en una pista, el sonido de la
  app y el del micrófono se mezclan al detener la grabación, que es lo que suena en cualquier
  reproductor. Separadas, cada fuente queda en su propia pista y su volumen se ajusta al editar;
  quien abra el archivo sin editar puede oír solo una.

## Las grabaciones

Los archivos quedan en `~/Movies/codeCanvas`, en `.mp4`, con el nombre por fecha y hora. **Abrir la
carpeta** la muestra en el Finder. La lista relee el disco al abrir el panel y al terminar una
grabación o una compresión.

Cada fila trae el nombre del archivo, la fecha y el tamaño, y los botones:

- **Assistir aqui no canvas**: abre la grabación en un panel de vídeo.
- **Abrir no player externo**: la abre en el reproductor predeterminado del Mac.
- **Comprimir o arquivo**: abre las opciones de compresión. Desaparece mientras otra compresión está
  en curso.
- **Mostrar no Finder**.
- **Apagar**.

**Dos clics en el nombre** entran en el modo de renombrar. La extensión se mantiene; un nombre vacío
o repetido se rechaza, y el campo sigue abierto.

### Comprimir

Una grabación por vez, con el progreso en su propia fila, y los botones de esa fila desaparecen
mientras corre.

- **Cuánto comprimir**: **Equilibrada** (un archivo grabado en Máxima se reduce en torno a 5×) o
  **Compacta** (la mitad de los bits de Equilibrada; el texto pequeño pierde definición).
- **Dónde guardar**: **Guardar como copia**, que es lo predeterminado y mantiene el original con la
  versión menor al lado, con "-comprimido" en el nombre; o **Sobrescribir el original**, que solo
  cambia el archivo con la compresión completa.

## Grabar sin abrir el panel

En **Configuración → Interfaz**, la opción **Barra de grabación en el pie** pone grabar, pausar,
detener y el tiempo en el pie de la app. Nace desactivada, y desactivarla no afecta al panel ni a
los comandos de voz.

Por voz: iniciar, pausar, retomar y detener la grabación, y poner la ventana en cualquiera de los
cuatro formatos.

Un agente puede listar las grabaciones existentes, con la fecha, el tamaño y la ruta de cada una.
Ver [el agente maneja el lienzo](o-agente-mexe-no-canvas).
