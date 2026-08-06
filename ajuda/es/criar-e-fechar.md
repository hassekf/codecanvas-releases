---
slug: criar-e-fechar
titulo: Crear y cerrar agentes
resumo: Abrir un agente, despedirlo, llamarlo de vuelta con la conversación, olvidarlo del todo, y qué pasa cuando duerme o se cae.
area: agentes
nivel: basico
---

## Crear

- **El botón de agente nuevo, en la barra de comandos**: abre el diálogo **Nuevo agente**.
- **`⌘N`**: crea un Claude Code directo, con el cursor ya dentro, incluso mientras escribes a otro
  agente. **`⇧⌘N`** crea un Codex, y solo funciona con Codex activado en **Ajustes → Proveedores**.
  Las dos teclas se cambian en **Ajustes → Atajos**.
- **El `⌘K`**: las entradas de agente nuevo, una por CLI activada, crean el agente directo, sin
  diálogo.
- **Por voz**: *"abre un agente"*, *"levanta tres agentes"*. Decir el nombre de un agente que ya
  existe nunca crea otro, aunque esté guardado.
- **Un agente**, cuando trae colegas al lienzo. Ver [un agente llama a otro](um-agente-chama-outro).

## El diálogo Nuevo agente

- **Herramienta**: en qué CLI nace el agente. Solo aparece con más de una activada.
- **Cuenta**: en qué instalación nace. Solo aparece si hay cuentas registradas para esa CLI, y vuelve
  a **La del proyecto** cuando cambias de herramienta. Ver [cuentas y perfiles](contas-e-perfis).
- **Nombre**: ya viene con una sugerencia. Hacer clic en el campo borra la sugerencia, y confirmar
  con el campo vacío la usa igual.
- La carpeta aparece abajo y no se edita aquí: es la del lienzo.

## Despedir

Cerrar el panel de un agente, con el botón de cerrar del encabezado o con la tecla Suprimir mientras
el lienzo tiene el foco, termina el proceso y quita el panel de la pantalla. El proyecto guarda el
nombre, la CLI, la cuenta, la última tarea, el asunto que el agente anotó, las entregas y la clave de
la conversación.

## Llamar de vuelta

- **En el panel de elenco**, con el botón **Llamar**. Ver [el panel del elenco](painel-elenco).
- **En el `⌘K`**, escribiendo su nombre.
- **Por voz**: *"llama a Hermes de vuelta"*. Mandarle una tarea a un agente guardado también lo trae.

Vuelve en la misma CLI y en la misma cuenta en que nació, y la conversación sigue donde quedó.

### Cuando la conversación no aparece

- Un agente que **nunca recibió un prompt** no tiene conversación grabada, y la app no avisa nada:
  vuelve nuevo.
- Un agente que **ya conversó** y cuya conversación no se encuentra genera un aviso que dice en qué
  cuenta buscó la app.
- Si la conversación está en **otra cuenta registrada**, el aviso dice cuál, y cambiar la cuenta de
  ese agente es lo que la trae. La app no copia nada entre cuentas por su cuenta.

## Olvidar

Olvidar es lo contrario de despedir: el agente sale del elenco, deja de poder llamarse de vuelta y su
nombre queda libre otra vez. La carpeta de la conversación sigue en el disco.

**Solo se olvida desde el [panel de reparto](painel-elenco)**, no desde el panel del agente. Ahí:

- **El botón de olvidar**, en cada fila guardada.
- **Olvidar todos**, en el encabezado de la sección **Guardados**, pide dos confirmaciones, porque
  esos tienen conversación.
- **Liberar nombres**, en el encabezado de **Guardados sin historial**, olvida de una vez a los que
  nunca recibieron un prompt.

## Agentes que duermen

En **Ajustes → Agentes**, **Hibernar agentes inactivos** viene desactivado. Activado, el agente sin
actividad por el tiempo definido en **Dormir después de** se cierra, el panel queda con un botón
**Despertar**, y la conversación se reanuda donde quedó cuando el agente vuelve. Lo que estaba
escrito en esa terminal hasta ahí se pierde.

- **Dormir después de** va de 5 minutos a 8 horas, y viene en 1 hora. El reloj se reinicia con cada
  herramienta que el agente usa, con cada prompt que envías y siempre que abres su panel.
- **Nunca duermen**: quien está trabajando, quien espera una respuesta tuya, y el panel seleccionado
  en el lienzo que estás viendo.
- **Enviar un prompt despierta al agente** y entrega el mensaje, sin pasar por el botón.

## Cuando la API tumba a un agente

El agente cortado a mitad de la respuesta entra en estado de caída, no en el de listo. La app te
avisa según tus [avisos y sonidos](avisos-e-sons).

Con **Reanudar agentes que la API tumbe** activado, que es el valor por defecto, la app le manda al
agente continuar desde donde quedó, explicando qué pasó. Los intentos siguientes esperan 3 segundos,
30 segundos, 1 minuto, 2 minutos y 5 minutos, y dejan de crecer ahí. Tras cuatro caídas seguidas la
app deja de insistir y pasa a esperar a que el proveedor vuelva. Reanudar solo no silencia el aviso.
El interruptor está en [configuración de los agentes](ajustes-agentes), y mandar continuar a mano
está en [hablar con ellos](falar-com-eles).
