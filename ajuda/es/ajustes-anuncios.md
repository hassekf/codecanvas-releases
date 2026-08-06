---
slug: ajustes-anuncios
titulo: Anuncios
resumo: Alertas visuales que tú diseñas y que los agentes de este proyecto disparan al cumplir una regla tuya: los campos, los marcadores y cuándo llegan a la pantalla.
area: projeto
nivel: basico
---

En la [configuración del proyecto](ajustes-projeto), sección **Anuncios**. La lista es de cada
lienzo.

## La lista

Cada fila muestra el icono, el nombre, el estilo y la regla de disparo, y trae:

- **El interruptor**: activa y desactiva. Desactivado, el anuncio sigue guardado y solo deja de
  dispararse.
- **El lápiz**: abre el anuncio en el editor de abajo. Hacer clic en la fila hace lo mismo.
- **La papelera**: elimina el anuncio.
- **Nuevo anuncio**: crea un anuncio vacío y lo abre en el editor.

## El editor

- **Nombre — cómo lo llama el agente**: la clave del anuncio. El agente dispara diciendo este
  nombre, y un nombre que no reconozca no dispara nada.
- **Cuándo disparar — la regla**: en lenguaje común. Es el **único** campo que el agente lee, y
  cuanto más específica sea la regla, menos se equivoca de momento.
- **Estilo**: **Level Up** (franja central, tres líneas de texto), **Píldora** (arriba, dos líneas,
  la menos intrusiva) o **Logro** (tarjeta lateral con el icono en un cuadrado, tres líneas).
- **Icono**: una cuadrícula de doce símbolos, y un campo para escribir el nombre de cualquier SF
  Symbol.
- **Texto de cada parte**: un campo por línea del estilo elegido. Cambiar de estilo no borra el
  texto que sobra, pero lo que sobra no se muestra.
- **Valores de prueba — lo que el agente rellenaría**: solo aparece cuando el texto tiene
  marcadores. Se usa únicamente en la simulación, y no se guarda.
- **Simular disparo**: llama al anuncio de verdad en tu pantalla, con los valores de prueba. Un
  marcador sin valor de prueba aparece con su propio nombre, y la simulación se salta la espera
  descrita abajo.

## Los marcadores

Un trozo entre llaves dentro del texto (`{versao}`, `{quantos}`) es un hueco que el agente rellena
al disparar. El nombre del marcador acepta letras, dígitos y `_`.

La plantilla `Release {versao} no ar` se convierte en "Release 1.48.1 no ar" cuando el agente
dispara pasando la versión. Un marcador sin valor queda en texto vacío: la clave nunca llega a la
pantalla.

El agente no escribe nada más. El estilo, el icono y las palabras fijas son tuyos; él dice qué
anuncio disparar y entrega los valores que faltan.

## Cuándo aparece el anuncio

El anuncio entra en la pantalla, se queda cerca de tres segundos y sale. **No** aparece mientras
estás en una reunión, hablando con la asistente, con el micrófono abierto o con la app hablando: en
esos casos entra en una cola y aparece en cuanto quedas libre. Ninguno se pierde.

Uno por vez, y el mismo anuncio disparado por varios agentes a la vez aparece una sola vez.

## Qué reciben los agentes

La lista de los anuncios **activos**, con nombre, regla y los marcadores a rellenar, entra en el
briefing de cada agente de este proyecto en el momento en que se crea. Un anuncio creado, renombrado
o activado después no llega a los agentes que ya están en marcha.

Un anuncio sin nombre o sin regla no entra en la lista, aunque esté activo.

No se le puede pedir un anuncio a la asistente por voz: quien dispara es el agente. Ver
[el agente maneja el lienzo](o-agente-mexe-no-canvas).

Para los avisos que da la propia app, que son otra cosa, ver [avisos y sonidos](avisos-e-sons).
