---
slug: quanto-custa
titulo: Cuánto cuesta la voz
resumo: Qué gasta créditos de OpenAI, qué pesa en la cuenta de la conversación, los dos techos y dónde ver el gasto.
area: nina
nivel: basico
---

En **Ajustes → Costos**. El gasto sale de los créditos prepagados de la cuenta de API cuya clave
guardaste en [Ajustes → Conversación](configurar-a-voz). La suscripción a ChatGPT no da acceso a la
API.

## Qué no gasta créditos

- **El dictado**: la transcripción ocurre en tu Mac. Ver [dictado](ditado).
- **La voz del sistema**: es la voz de macOS, y es la que habla cuando la voz natural está apagada.
- **La escucha que se abre después de un aviso hablado**: usa el reconocimiento local. Quedarte
  callado en ella no gasta nada.
- **[La conversación escrita](a-nina-por-texto)** (⌘J): responde con el CLI de agente que ya pagas.

## Qué gasta créditos

- **La conversación por voz** (⌥C): audio de ida y de vuelta. Es el elemento más caro.
- **[El modo comando](o-modo-comando)** (⌥X): solo texto, porque la transcripción se hace en tu Mac.
- **La voz natural**: los avisos hablados y las confirmaciones del comando.
- **El saludo de la mañana**: la frase la escribe un modelo cuando hay clave; sin clave, la app arma
  la frase sola y no gasta nada.
- **La generación de imágenes y el papel tapiz pedido por voz**. La calidad elegida cambia bastante el
  precio. Ver [la galería](painel-galeria).

## Qué pesa en la cuenta de la conversación

- **El audio que ella habla** es el elemento más caro de todos, y nunca se reaprovecha.
- **Cada respuesta reprocesa la sesión entera**: las instrucciones, las herramientas y el historial.
  La cuenta sube con la duración de la conversación, no con el volumen de tu voz.
- **Las herramientas activas entran en ese reprocesamiento.** En **Ajustes → Herramientas**, la
  bloque de arriba muestra el costo aproximado de cada intercambio con la selección actual, y cuántos
  intercambios por minuto caben en el límite de tu cuenta; cada grupo muestra cuánto cuesta. Apagar un
  grupo quita sus herramientas de la conversación y no deshace la integración.

## Los dos techos

En Ajustes → Conversación.

- **Cerrar tras silencio**: cierra después de ese tiempo sin que nadie hable. Predeterminado 90
  segundos, cero lo desactiva.
- **Tiempo máximo de la conversación**: cierra al terminar el tiempo incluso mientras hablas, y es el
  único que garantiza un límite de gasto por conversación. Predeterminado 5 minutos, cero es sin
  techo.

## El modelo

- **Modelo de Nina**: el modelo de la conversación por voz, y el precio cambia con él. La lista viene
  de tu cuenta, y el botón "Actualizar" la rehace. La app elige el primero de la lista cuando el
  modelo guardado deja de estar disponible.
- **Modelo del comando** (Ajustes → Voz): el modelo que interpreta las órdenes habladas.

## Dónde ver el gasto

En Ajustes → Costos:

- **Gasto de esta sesión**: el total de la conversación abierta ahora, con el número de turnos y el
  reparto entre texto y audio, sacados de lo que el servicio cobró turno a turno. El botón **Abrir el
  resumen** muestra en el Finder el archivo del día, guardado en Application Support/codeCanvas/voz.
- **Hoy** y **Total**, con el número de llamadas al lado.
- **Últimos 14 días**: el gráfico por día.
- **Por modelo**: llamadas, tokens y costo de cada uno. Una fila marcada con el signo de aproximación
  es una estimación: la API de voz no informa el consumo, y el valor se calcula por los caracteres
  hablados.
- **Limpiar resumen**: borra los números de aquí. El cobro ya hecho sigue en OpenAI.

Los valores por debajo de un centavo se muestran con cuatro decimales, en lugar de volverse cero.
