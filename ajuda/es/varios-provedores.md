---
slug: varios-provedores
titulo: Varias CLIs de agente
resumo: Claude Code, Codex, Grok y opencode en el mismo lienzo: cómo activarlas, qué funciona igual en todas y qué es de una sola.
area: agentes
nivel: basico
---

En **Ajustes → Proveedores**, **CLIs de agente** tiene una fila por CLI: Claude Code, Codex, Grok y
opencode.

- **El estado de la fila**: **instalado**, con el nombre del ejecutable al lado, o **no encontrado en
  el PATH**. La app busca cada uno en el `PATH` de tu shell.
- **El interruptor**: activa la CLI. Una CLI que no está instalada y no está activada no se puede
  activar, y desactivar la última activada no tiene efecto.
- **El comando de instalación**: aparece en la fila de la que no se encontró, con un botón que lo
  copia. La app no instala ni actualiza CLIs de terceros. La excepción es Claude Code, que el panel
  de un agente ofrece instalar en un clic cuando falta.

Una CLI activada pasa a aparecer en los tres lugares donde nace un agente: en el `⌘K`, con una
entrada de agente nuevo por CLI, en la barra de comandos y en la voz, que acepta las grafías que la
transcripción produce para sus nombres.

## Qué es igual en todas

- El panel con la terminal de la CLI, y su nombre en el encabezado, junto al nombre del agente.
- Los estados de cada panel y los avisos: trabajando, esperándote, listo, se cayó, finalizado.
- El reverso del panel, con el asunto que el agente escribe sobre sí mismo y el historial de
  entregas.
- La autoría por archivo, antes del commit. Ver [el panel de Git](painel-git).
- Despedir y llamar de vuelta con la conversación. Ver [crear y cerrar](criar-e-fechar).
- Las herramientas del lienzo: el navegador propio, abrir paneles, leer lo que otro agente está
  haciendo y traer colegas.

## Qué es de una sola CLI

- **Elegir la opción de una pregunta hablando** vale para las preguntas de opción múltiple de Claude
  Code. En las demás, la pregunta se lee igual y la respuesta va como texto, escrito o dictado.
- **Instalar y fijar la versión** es de Claude Code. El menú **Versión de Claude Code**, en
  **Ajustes → Agentes**, fija una de las versiones presentes en la máquina y, mientras esté fijada,
  desactiva la actualización automática.
- **Registrar instalaciones** pide una carpeta `.claude`, en **Instalaciones de Claude**, en la misma
  pantalla. Un agente elige entre ellas al crearse y en el menú contextual del panel. Ver
  [cuentas y perfiles](contas-e-perfis).
- **El modelo de opencode se elige dentro de él**: los modelos que corre dependen de las cuentas en
  las que iniciaste sesión, y el lienzo no le pasa ningún modelo. En las demás, el modelo por defecto
  del lienzo se elige en [ajustes del proyecto](ajustes-projeto).

## Cambiar la CLI de un agente

El menú contextual del panel no cambia la CLI de un agente existente: cada agente vive en la CLI en
que nació, incluso cuando se lo llama de vuelta después de despedirlo. Lo que el menú ofrece es
cambiar su **cuenta**, dentro de la misma CLI.
