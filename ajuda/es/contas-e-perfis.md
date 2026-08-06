---
slug: contas-e-perfis
titulo: Cuentas y perfiles
resumo: Dónde se registran las instalaciones del programa de agente, en cuál nacen cada proyecto y cada agente, y qué pasa con la conversación al cambiar.
area: agentes
nivel: basico
---

Una cuenta es una carpeta de configuración del programa de agente. El inicio de sesión, los ajustes y
las conversaciones de los agentes viven dentro de ella, y por eso la cuenta decide de qué memoria
dispone un agente.

## La lista de cuentas

En **Ajustes → Agentes → Instalaciones de Claude**.

- **La instalación predeterminada**: la carpeta que tu terminal ya usa. Siempre está en la lista y no
  se puede quitar.
- **Renombrar**: cambia el nombre de una cuenta. Ese nombre aparece en el encabezado de cada agente
  que nace en ella, y solo cuando hay más de una cuenta registrada. Un nombre vacío devuelve la
  etiqueta original.
- **Agregar instalación…**: abre el selector de carpetas, con los elementos ocultos a la vista, y
  registra la carpeta elegida. No se copia nada: la app pasa a apuntar a ella. El nombre sugerido
  viene de la carpeta que contiene a la elegida cuando el nombre de esta empieza con punto. La misma
  carpeta no entra dos veces.
- **Quitar de la lista**: da de baja la cuenta. Si algún agente nace en ella, la app pregunta antes y
  ofrece **Llevar las conversaciones a la predeterminada** o **Quitar y dejar las conversaciones
  ahí**. Nada se borra del disco en ninguno de los dos casos, y las conversaciones vuelven si
  registras la carpeta de nuevo.

Cada fila muestra la ruta de la carpeta y su estado: una carpeta nunca usada avisa de que el primer
agente pedirá el inicio de sesión, y una carpeta que salió del disco se señala como desaparecida.

El programa de agente de una cuenta se deduce del contenido de la carpeta, no lo eliges tú. Una
cuenta pertenece a un solo programa. Ver [varios programas de agente](varios-provedores).

## La cuenta del proyecto

En **Editar el proyecto → Agentes → Instalación de Claude**. Con una sola cuenta registrada, el menú
trae la predeterminada y la instrucción de registrar las demás en Ajustes.

- **La elección vale para todo el canvas**: cada agente que nazca ahí usa esa cuenta, salvo los que
  hayan elegido la propia.
- **Al guardar un cambio con agentes abiertos**, la app pregunta entre **Llevar las conversaciones**
  y **Empezar de cero en la cuenta nueva**, y los agentes que heredan la cuenta del proyecto renacen
  en ella. La conversación vuelve entera; el turno en curso en ese instante se pierde. Quien eligió
  su propia cuenta no se toca.
- **Si la carpeta elegida ya no existe**, la pantalla avisa ahí mismo: el agente nacerá sin sesión
  iniciada.

## La cuenta de un agente

En el menú del panel del agente, en **Cuenta de ‹nombre›**. El elemento solo aparece cuando hay otra
cuenta registrada del mismo programa de agente.

- **Las opciones** son la cuenta del proyecto, la instalación predeterminada y cada cuenta
  registrada. La actual viene marcada y no se puede volver a elegir.
- **Elegir no cambia nada de inmediato**: abre una pregunta. Si el agente ya conversó, ofrece
  **Llevar la conversación** o **Empezar de cero allí**; si nunca conversó, solo **Cambiar**.
- **Llevar la conversación** copia su pasado dentro de la carpeta de la cuenta nueva, y vuelve
  recordándolo todo. Empezar de cero mantiene las dos cuentas separadas en el disco. La conversación
  antigua no se borra en ninguno de los dos casos.
- **La elección es de ese agente**: cambiar después la cuenta del proyecto no lo arrastra.
- **El agente renace en la cuenta nueva**, con el mismo nombre y el mismo lugar en el canvas. Lo que
  estuviera haciendo en ese instante se pierde.

## Cuando un agente vuelve sin la conversación

La conversación vive dentro de la carpeta de la cuenta. Llamar de vuelta a un agente en una cuenta
distinta de aquella en la que trabajó lo trae con el nombre correcto y la memoria en blanco.

La app avisa en ese caso y dice en qué cuenta buscó. Si la conversación está en otra cuenta
registrada del mismo programa, dice en cuál, y no la trae: traerla es el cambio de cuenta descrito
arriba.

## Configurado en otra pantalla

- Los programas de agente disponibles: [varios programas de agente](varios-provedores).
- Cómo nacen los agentes de este canvas: [ajustes del proyecto](ajustes-projeto).
- Llamar de vuelta a un agente guardado: [crear y cerrar agentes](criar-e-fechar).
