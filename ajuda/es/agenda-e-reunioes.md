---
slug: agenda-e-reunioes
titulo: Agenda y reuniones
resumo: Conectar el calendario del Mac, qué puede ver Nina de él, el aviso antes de la hora y el modo reunión.
area: integracoes
nivel: basico
---

En **Ajustes → Integraciones**. CanvasCode lee el Calendario del Mac, con todas las cuentas que ya
están en él, y nunca escribe nada en tu agenda.

## Conectar

- **Conectar la agenda**: activa la integración. macOS pide el permiso en ese momento. Si niegas el
  permiso, el interruptor vuelve a apagado, y la sección muestra un botón que abre Privacidad y
  Seguridad → Calendarios en los Ajustes del Sistema, porque macOS no vuelve a preguntar por su
  cuenta.

Activada, la tarjeta muestra cuántas citas hay hoy. Apagada, la integración no deja rastro: ningún
bloque en la pantalla de inicio, ningún aviso, y Nina no recibe nada sobre el tema.

- **Qué agendas entran**: marca y desmarca cada calendario del Mac. Ninguna marcada quiere decir
  todas.

## Qué puede ver Nina

Cinco elementos, activados de forma predeterminada, que deciden qué sube a OpenAI cuando le preguntas
a Nina por la agenda:

- **El título**: sin él, ella solo sabe que existe una cita.
- **El lugar**: la sala, la dirección, el edificio.
- **La descripción y el orden del día**: el cuerpo de la invitación.
- **Los participantes**: quién fue invitado y quién confirmó.
- **El enlace de la llamada**: la dirección de Meet, Zoom o Teams. Sin él no puede abrir la llamada
  por voz.

La hora siempre acompaña a la cita, marques lo que marques. Los avisos, el bloque del día y las
notificaciones en pantalla se arman en tu Mac y no pasan por OpenAI, al margen de estos cinco.

El grupo entero de herramientas de agenda también se apaga en Ajustes → Herramientas: Nina deja
entonces de leer el calendario y de entrar en llamadas, y la integración sigue conectada.

## Tu día en la pantalla de inicio

Debajo de los proyectos aparece un bloque con las citas de hoy, o las de mañana cuando hoy ya no tiene
ninguna. La cabecera dice cuál de los dos días se está mostrando.

- Lo que ya pasó se queda en la lista, atenuado; lo que está ocurriendo aparece marcado como "agora".
- Al pasar el ratón por una reunión con enlace aparece el botón de entrar.
- Al hacer clic en la fila se abre el detalle: hora, calendario de origen, participantes, orden del
  día y un botón **Abrir en Calendario**, que es donde se crean, se mueven y se cancelan las citas.

## El aviso antes de la hora

- **Avisar antes de la reunión**: muestra una notificación antes de que la reunión empiece. No
  desaparece sola.
- **Avisar antes**: cuántos minutos antes, entre 5, 10, 15 y 30. El predeterminado es 10.

El aviso es de una reunión por vez, siempre la próxima que aún no ha empezado. En una reunión con
enlace ofrece los dos caminos de entrada, el de tu preferencia primero y el otro al lado, más un botón
que lo descarta. El aviso se va solo una hora después del final de la reunión, o en el instante en que
se cancela en el calendario.

- **Al abrir una reunión**: elige entre "En un panel de aquí" y "En mi navegador". Aquí dentro, Meet
  abre con la sesión de Google que los paneles de navegador ya usan.

Al entrar por un panel de aquí, la llamada se vuelve el centro de la pantalla si el lienzo se organiza
solo. Con los paneles ordenados a mano, nada se mueve de sitio.

## El modo reunión

Entrar en una llamada desde el aviso, por voz o desde el botón activa el modo reunión. Con él
activado:

- No se habla nada y no aparece ninguna notificación.
- El micrófono no se abre solo después de un aviso.
- **Las teclas de dictado, comando y conversación no abren el micrófono.** Pulsar una de ellas muestra
  una notificación diciendo que el micrófono está con tu reunión, con el botón de salir al lado.
- La conversación por voz que estuviera abierta se cierra al entrar.

El distintivo de la barra muestra "En reunión" y es la salida: al hacer clic en él, el modo se apaga.
El modo también sale solo cinco minutos después del final de la cita, y sale cuando cierras el panel
en el que la llamada se había abierto.

Por voz, "fica quieta um pouco" activa el modo sin ninguna reunión, y "acabou a reunião" lo apaga.

### Nada se pierde

Lo que llegaría durante la reunión queda guardado. Al salir, los avisos que describen un problema aún
vivo, como un agente caído, vuelven enteros; los demás se convierten en una notificación que dice
cuántos llegaron, con un botón **Ver** que abre el historial.

## Por voz

```
"o que eu tenho hoje?"           "qual a próxima reunião?"
"do que é a reunião das três?"   "quem vai estar nela?"
"entra na reunião"               "abre o Meet"
"fica quieta um pouco"           "acabou a reunião"
```

Las órdenes se interpretan en portugués. Sin decir cuál, ella entra en la que está ocurriendo o en la
próxima en empezar. No hay forma de crear, mover ni cancelar una cita por voz.

## En el saludo de la mañana

- **Hablar de las reuniones** (Ajustes → Saludo): incluye las citas de hoy en el saludo de la mañana,
  en la misma frase que las demás pendencias. Ver [hablar con Nina](falar-com-a-nina).
