---
slug: ajustes-mcp
titulo: Ajustes · MCP
resumo: La pantalla que elige los servidores MCP que levantan los agentes de este proyecto, instala nuevos desde el registro oficial y dice lo que cuesta cada uno.
area: projeto
nivel: avancado
---

En **Editar el proyecto → MCP**.

## Instalados desde aquí

Los servidores que vinieron del registro, por CanvasCode.

- **El interruptor** activa el servidor en este canvas. Cada servidor instalado nace activo solo en
  el canvas desde el que partió la instalación, y dormido en los demás.
- **Desinstalar…**, en el menú de la fila: saca el servidor del acervo de la app.

## Ya configurados

Los servidores que instalaste por fuera, en tu cuenta del programa de agente o en el propio proyecto.
CanvasCode no los modifica: aquí solo eliges usarlos o no en este canvas.

- **Todos vienen activados.** Desactivar uno deja de levantarlo para los próximos agentes de este
  proyecto.
- **Volver a activarlos todos** regresa al estado de heredar la lista entera, y un servidor nuevo que
  configures por fuera entra solo.
- **Sin ningún servidor configurado por fuera**, la sección lo dice.

## Lo que cuesta cada uno

Cada fila lleva una etiqueta.

- **HTTP**: el servidor es compartido y no cuesta nada por agente.
- **Proceso**: levanta un proceso por agente, unos 60 MB cada uno. Con seis agentes en pantalla, son
  seis.

El servidor MCP del propio CanvasCode, el que le da al agente los paneles, el navegador y tus listas,
queda fuera de esa cuenta: es uno solo, dentro de la app, compartido por todos los agentes.

## Instalar

**Instalar…**, arriba, busca en el registro oficial, que es público y no pide cuenta.

- **Cada resultado** dice si el servidor habla por HTTP o levanta un proceso, y si pide clave.
- **La confirmación** muestra el costo, el enlace al código fuente y los campos que necesita, con los
  obligatorios marcados. El botón de instalar queda no disponible mientras falte un obligatorio.
- **Las claves van al Keychain de tu Mac**, nunca a un archivo, y se le entregan al servidor solo en
  el momento de levantar el agente.
- **Instalado desde un proyecto**, el servidor queda activo en él y dormido en los demás.

## Guardar reinicia a los agentes parados

Un agente no relee sus propios argumentos una vez nacido. Al guardar un cambio de servidores, los
agentes parados de este canvas renacen con la lista nueva, y la app te dice cuáles fueron.

- **Renacer no es empezar de nuevo**: vuelven con la conversación entera y el mismo lugar en el
  canvas. Lo que se pierde es el historial ya pintado en la pantalla de la terminal.
- **A quien está trabajando no se lo toca.** Esos agentes toman los servidores nuevos la próxima vez
  que renazcan.

## Configurado en otra pantalla

- Qué es un servidor MCP, y qué se le puede pedir a un agente: [skills y servidores MCP](skills-e-mcp).
- Las instrucciones que cargan los agentes: [Ajustes · Skills](ajustes-skills).
