---
slug: ditado
titulo: Dictado
resumo: ⌥D y hablar: adónde va el texto, qué se vuelve símbolo, los dos motores y el dictado largo.
area: nina
nivel: basico
---

**⌥D** dicta a un agente. La tecla se cambia en **Ajustes → Atajos**, en la fila "Ditar", y el motor
de transcripción se elige en **Ajustes → Voz**.

El texto llega al agente palabra por palabra, sin ningún modelo reescribiendo lo que dijiste.

## La tecla

- **Mantener y soltar**: la app escucha mientras la tecla está pulsada; al soltar, envía.
- **Tocar y soltar**: la escucha queda fijada y hablas a tu ritmo. La ventanita pasa a decir "toca de
  nuevo para enviar", y es ese toque el que envía.
- **Esc**: cancela. El texto se descarta y no llega a ningún agente.

Con la escucha fijada, un minuto de silencio pausa el dictado. Lo que dijiste queda guardado en una
aviso con tres salidas: **Seguir hablando**, **Enviar** y **Descartar**. Sin un agente elegido, el
aviso te pide que hagas clic en el panel de quien va a recibirlo, y el envío queda no disponible
hasta entonces.

## Adónde va el texto

Las reglas son fijas, sin ningún modelo decidiendo:

- **"Peça pro Marshall extraia o guard clause pro topo"**: va literal a Marshall. Reconoce varias
  formas de dirigirse ("peça pro", "pede pro", "manda pro", "fala pro", "diz pro", "ei") y quita el
  nombre y los conectores del principio del texto.
- **"Foco no Marshall"**: destaca su panel, sin enviar texto.
- **Cualquier otra frase**: va al agente seleccionado. Con un único agente en el lienzo, va a ese.
- **Con [la conversación escrita](a-nina-por-texto) abierta**: cae en su campo.

El nombre se reconoce ignorando acentos y mayúsculas. La ventanita del dictado muestra el destino al
lado del texto, o "sem destino" cuando no hay a quién mandarlo. **Un archivo seleccionado en el lienzo
viaja junto con el texto**, como referencia delante de lo que dictaste, y la ventanita lo marca al
lado del nombre del destinatario.

- **Hilo del dictado** (Ajustes → Interfaz): activa el hilo que va de la barra del dictado hasta el
  panel que va a recibir el texto. Apagado, el destino sigue escrito al lado de la barra.

## La puntuación dictada

Cuatro palabras se vuelven símbolo cuando están entre dos piezas que parecen un identificador:

- **"underline"** y **"sublinhado"** se vuelven `_`.
- **"barra"** se vuelve `/`. "Src barra components" se vuelve `src/components`.
- **"hífen"** se vuelve `-`.
- **"ponto"** se vuelve `.` solo antes de una extensión de archivo conocida. "Index ponto tsx" se
  vuelve `index.tsx`; "até que ponto é viável" queda tal como lo dijiste.

La conversión no ocurre cuando uno de los lados es una palabra común, como en "na nossa barra aqui
embaixo". Fuera de eso, el dictado no toca tu puntuación y no corrige tu texto.

## Los dos motores

En Ajustes → Voz → Modelo de transcripción.

- **Sistema (Apple)**: ya viene en macOS y muestra el texto mientras hablas. Es el predeterminado.
- **Parakeet v3**: descarga unos 600 MB, una sola vez, desde el botón del propio bloque, y funciona
  en tu Mac sin internet. Transcribe cuando **sueltas** la tecla: mientras hablas la ventanita muestra
  "ditando…", y el texto llega al final.

El dictado sigue el idioma elegido para la app. Lo que sigue entendiendo solo portugués son las
órdenes habladas del [modo comando](o-modo-comando).

## Dictado largo

En **Ajustes → Diagnóstico**, cuatro interruptores que valen solo para Parakeet y solo para hablas de
más de unos quince segundos. Todos nacen activados.

- **Evitar el cambio de idioma**: impide que el texto se deslice al inglés en medio del portugués.
- **Recuperar fragmentos perdidos**: reconstruye palabras comidas en la unión entre las ventanas del
  dictado.
- **Cortar el habla larga en fragmentos**: divide el audio en los silencios y transcribe cada
  fragmento aparte. Deja el habla larga un poco más lenta.
- **Anclar el idioma en cada fragmento**: pone una palabra del idioma delante de cada fragmento y la
  quita del texto final.

## Mandarlo de nuevo a otro agente

```
"aquilo da migração, joga pro Hermes"
"mandei errado, reenvia o último pro Apolo"
```

La app busca en el historial lo que ya dictaste y se lo entrega al otro agente, sin que repitas la
frase. Es una petición de voz, así que vale por ⌥C o por ⌥X.

## Límites

- El dictado y la conversación se disputan el mismo micrófono: abrir la conversación con la tecla del
  dictado pulsada se rechaza, con aviso.
- En [modo reunión](agenda-e-reunioes) el dictado no abre el micrófono, y la app muestra una
  notificación diciendo que está con la llamada.
