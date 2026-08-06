---
slug: iniciativas-o-que-e
titulo: Qué es una Iniciativa
resumo: El proceso de trabajo del equipo escrito en un archivo del repositorio, que CanvasCode lee, dibuja y conduce.
area: iniciativas
nivel: avancado
---

Una **Iniciativa** es el proceso que tu equipo ya sigue, escrito en un archivo del repositorio: las
etapas en orden, quién hace cada una, qué bloquea, y dónde aprueba una persona. CanvasCode lee ese
archivo, dibuja el proceso y conduce las ejecuciones.

**La app no implementa el proceso de nadie.** Quien ejecuta siguen siendo los comandos, los scripts y
los agentes que el proyecto ya tiene. El archivo es una lente sobre ellos, y si él y los comandos no
coinciden, ganan los comandos.

## El vocabulario

| Palabra | Qué es |
|---|---|
| **Iniciativa** | El proceso definido, en un archivo dentro del repositorio |
| **Ejecución** | Una ejecución de ese proceso, de principio a fin |
| **Paso** | Una etapa: un agente o un comando, con lo que entra y lo que sale |
| **Puerta** | Un comando que prueba que el resultado del paso sirve |
| **Revisión** | Un paso cuya salida es un veredicto, y cuyo efecto es cambiar la ruta |

## Para qué sirve

Para el trabajo que se repite y tiene orden: una cadena de contenido, un flujo de release, una
investigación que siempre pasa por las mismas cinco etapas con una aprobación tuya en medio.

No sirve para una tarea suelta. Para pedirle una cosa a un agente, el camino sigue siendo su panel o
la voz.

## Qué cambia respecto a mandarlo tú mismo

- **El orden no se pierde.** Cada paso recibe lo que produjo el anterior, y un resumen de hasta tres
  líneas con lo que el artefacto no dice: el riesgo que vio el agente y la decisión que tomó.
- **Quien dice que el paso terminó es la puerta, no el agente.** El agente avisa que cree que
  terminó; la app ejecuta el comando que lo prueba, y si rechaza, el trabajo vuelve con el motivo.
- **Quien revisa es siempre un agente nuevo**, porque revisar el propio trabajo con la conversación
  todavía en la cabeza es la revisión más floja que existe.
- **Quien corrige es el mismo agente en la primera vuelta**, y un agente nuevo a partir de la
  segunda.
- **Todo bucle tiene tope.** Y un artefacto idéntico al de la vuelta anterior se detiene al momento,
  sin gastar la vuelta siguiente.
- **Ningún agente se activa sin que tú elijas cuál.** Todo botón que habla con un agente abre el
  selector antes y muestra lo que se va a mandar.

## Dónde están los archivos

- **La Iniciativa** está en `.codecanvas/iniciativas/` dentro del repositorio, y se versiona con el
  código: viaja hasta quien clone el proyecto.
- **Las ejecuciones** están en `.codecanvas/runs/`, fuera de git: son ejecución, no definición.

**Una Iniciativa es por repositorio.** Está hecha de los comandos y los scripts de ese proyecto, y no
se reaprovecha en otro.

## Qué se puede hacer en paralelo

Dentro de una ejecución, todo es cola: un paso, un agente, una entrada, una salida. El paralelismo
existe un nivel más arriba, en dos ejecuciones de la misma Iniciativa a la vez, para comparar
resultados.

## Por dónde seguir

- Escribir una: [escribir una Iniciativa](iniciativas-escrever).
- Seguir las ejecuciones: [el panel de Iniciativas](painel-iniciativas).
