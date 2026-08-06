---
slug: atualizacoes
titulo: Actualizaciones
resumo: La comprobación automática, el botón para buscar ahora, qué pasa con los agentes al instalar y las novedades de cada versión.
area: conta
nivel: basico
---

La app busca versión nueva sola, en segundo plano, cada hora, y al arrancar cuando ya pasó ese
intervalo desde la última vez.

## Pedirlo ahora

Dos puertas, y las dos hacen lo mismo:

- **El menú de la app → Buscar actualizaciones…**
- **Buscar actualizaciones**, en el pie de la Configuración, al lado del número de versión. Cierra la
  Configuración antes de comprobar, y no está disponible mientras hay una comprobación en curso.

La comprobación que pides responde incluso cuando no hay nada nuevo. La automática es silenciosa.

## Los agentes que están trabajando

- **La comprobación automática no ofrece actualización mientras haya un agente trabajando.** No
  insiste y no descarga nada: la siguiente comprobación vuelve a buscar y ofrece la versión más
  reciente de entonces.
- **La comprobación que pides sigue igualmente.** Al mandar instalar con alguien trabajando, la app
  lista por nombre a quien va a ser cerrado y ofrece **Adiar** (posponer) o **Instalar mesmo assim**
  (instalar de todos modos).
- **Posponer deja la actualización descargada esperando.** Mientras no se instale, es esa la versión
  que se vuelve a ofrecer, y las más nuevas no aparecen.
- La sesión de cada agente queda guardada y puedes llamarlos de vuelta por su nombre. Lo que estén
  haciendo en el instante de la instalación se pierde.

## Las novedades

- **Novedades**, en el pie de la pantalla de inicio: abre lo que cambió, versión a versión, con la
  tuya marcada.
- **El punto al lado del botón**: se enciende cuando hay una versión que aún no has leído, y se apaga
  cuando abres la lista.

La lista está escrita para quien usa la app. La parte técnica de cada versión queda fuera de ella.

## Por qué puedes confiar en lo que descarga

Cada actualización está firmada, y la app rechaza cualquier archivo cuya firma no coincida con la
clave que lleva. Además, el binario descargado sigue pasando por la comprobación de Apple, que es lo
que hace que la app abra sin el aviso de desarrollador no identificado. Ve [instalar](instalar).

## Cuando no actualiza

En el orden en que suele pasar:

1. **Sin internet, o una red que bloquea el acceso.** Pídelo por el botón para ver la respuesta.
2. **Siempre hay alguien trabajando.** Usa el botón e instala cuando puedas cerrar los agentes.
3. **Una actualización pospuesta, esperando.** Instálala, y las siguientes vuelven a llegar.
4. **Nada de eso.** Descarga la app de nuevo e instálala encima. Los lienzos, las conversaciones y la
   configuración no viven dentro de la app: ve [dónde están mis datos](onde-ficam-meus-dados).
