---
slug: configurar-a-voz
titulo: Configurar la voz
resumo: La clave de OpenAI, el micrófono, quién habla contigo, los timbres y las teclas de la voz.
area: nina
nivel: basico
---

En **Ajustes → Voz**. La clave y los ajustes de la conversación están en **Ajustes → Conversación**.

## La clave de OpenAI

En Ajustes → Conversación.

- **Clave de OpenAI**: guarda la clave en el Llavero de macOS. El valor junto al título muestra
  "configurada" o "falta", y la clave nunca se vuelve a mostrar. Al guardarla, la app busca los
  modelos que tu cuenta tiene, para la conversación y para las imágenes.

Sin clave quedan no disponibles Nina, la voz natural y el modelo del comando. El dictado, la voz del
sistema y [la conversación escrita](a-nina-por-texto) no dependen de ella.

## El micrófono

- **Modelo de transcripción**: elige cómo tu habla se convierte en texto. "Sistema (Apple)" es el
  predeterminado y muestra el texto mientras hablas. "Parakeet v3" descarga unos 600 MB una sola vez
  y transcribe cuando sueltas la tecla. Ver [dictado](ditado).
- **Micrófono**: elige el dispositivo de entrada. "Predeterminado del sistema" sigue a los Ajustes
  del Sistema y dice entre paréntesis cuál es ese dispositivo. Un dispositivo elegido y luego
  desconectado aparece como desconectado, en lugar de cambiarse en silencio.
- **Ganancia del micrófono**: multiplica la señal de entrada, de 1× a 24×. El valor predeterminado es
  1×.
- **Probar el micrófono**: muestra el audio que llega, ya con la ganancia aplicada, y marca con una
  línea el umbral a partir del cual se detecta el habla. El medidor sigue a la ganancia mientras
  arrastras el control, y deja de grabar cuando cierras los Ajustes.
- **Salida de audio**: elige el dispositivo de salida. La app todavía no usa esta elección.

## Quién habla contigo

Los tres interruptores de esta tarjeta funcionan en cascada: la app habla con la voz natural; cuando
esta no puede, con la voz del sistema; sin las dos, no habla.

- **Nina**: activa la conversación por voz (⌥C), el saludo de la mañana y la respuesta hablada a los
  agentes. No disponible sin la clave.
- **Voz natural**: usa la voz de OpenAI en los avisos y en las confirmaciones del modo comando. No
  disponible sin la clave.
- **Voz del sistema**: usa la voz de macOS, sin clave y sin internet. Es la que habla cuando la voz
  natural no puede.

Con los tres apagados, la tarjeta muestra "silencio" y todo lo que se hablaría se convierte en una
notificación en pantalla. El dictado sigue funcionando: es transcripción, no habla.

## Los avisos hablados

En Ajustes → Voz. Valen para los avisos y para la confirmación del modo comando, no para Nina.

- **Volumen de la voz**: del 10% al 100%, predeterminado 70%. Afecta solo a la voz de la app, no al
  volumen del Mac.
- **Velocidad de los avisos**: de 0,80× a 1,60×, predeterminado 1,00×. Por encima de 1,4× la voz
  empieza a comerse el final de las palabras.
- **Timbre**: elige la voz de la nube. El botón "Escuchar" reproduce una muestra por el mismo camino
  de un aviso real, con el volumen y la velocidad elegidos. No disponible con la voz natural apagada.
- **Modelo de la voz**: elige el modelo de síntesis. No disponible con la voz natural apagada.
- **Modelo del comando**: elige quién interpreta la frase del [modo comando](o-modo-comando). Depende
  de la clave, no de la voz natural: trabaja incluso con la app muda.

## La voz de Nina

En Ajustes → Conversación. Estos valen solo para la conversación por voz.

- **Modelo de Nina**: el modelo de la conversación. El botón "Actualizar" rehace la lista a partir de
  tu cuenta.
- **Voz de Nina**: su timbre, con un botón "Escuchar" que reproduce la muestra sin abrir conversación.
  El predeterminado es Marin.
- **Velocidad de Nina**: de 0,80× a 1,60×, predeterminado 1,00×.
- **Nombre de la asistente**: cómo la llamas, y cómo se presenta entre los agentes. El predeterminado
  es Nina.
- **Silencio para que responda**: cuánto silencio espera antes de dar por terminado lo que dices. De
  300 a 3000 ms, predeterminado 900 ms.
- **Sensibilidad del micrófono**: a partir de qué volumen el sonido cuenta como voz. De 0,10 a 0,90,
  predeterminado 0,50.

## Las teclas

Los valores de fábrica:

- **⌥D**: [dictar](ditado) a un agente.
- **⌥X**: [mandar al lienzo que actúe](o-modo-comando).
- **⌥C**: abrir y cerrar [la conversación por voz](falar-com-a-nina).
- **⌘J**: abrir y cerrar [la conversación escrita](a-nina-por-texto).
- **Esc**: cancela lo que esté en marcha, sea el dictado, el comando, la conversación o la voz que
  está hablando. El texto de un dictado cancelado se descarta y no llega a ningún agente.
- **⌥F**: gira los paneles y muestra el resumen de cada agente.
- **⌥O**: ordena los paneles sin superposición.

Todas se cambian en **Ajustes → Atajos**: haz clic en el campo de la fila y pulsa la combinación
nueva. La pantalla avisa cuando dos acciones quedan en la misma tecla, y dice cuáles son; en ese caso
una de las dos deja de funcionar. El Espacio se evita en los atajos de voz porque Claude Code ya usa
"mantener espacio" para dictar dentro del terminal.

Las teclas de voz valen con CanvasCode delante, incluso con el cursor dentro de un agente. Con la app
detrás de otra ventana, la tecla es de la app que estás usando. La excepción es Esc, que vale en todo
el Mac mientras hay voz en marcha.

**Mientras los Ajustes están abiertos, las teclas de voz no se disparan.** Vuelven, ya con los valores
nuevos, cuando la hoja se cierra, por cualquier camino.

## Cuando hablas y no pasa nada

- Una señal demasiado débil nunca cruza el umbral de detección: sube la **ganancia del micrófono**
  hasta que la prueba registre tu habla a volumen normal.
- El ruido de la sala que nunca deja silencio impide que el turno se cierre, y Nina no responde: sube
  la **sensibilidad del micrófono**. Si se come el inicio de tus frases, bájala.
- El micrófono depende del permiso de macOS. En **Ajustes → Diagnóstico** están el estado de cada
  permiso, el botón que lo pide de nuevo y otro que borra el registro de permisos de esta app para que
  el sistema pregunte desde cero, con la app reabierta después. Ver
  [los permisos que pide macOS](permissoes-do-mac).
