---
slug: o-que-e-um-agente
titulo: Qué es un agente
resumo: Una CLI de agente corriendo en una terminal de verdad dentro del panel, en la carpeta del lienzo, con nombre propio.
area: agentes
nivel: basico
---

Un agente es una CLI de agente (Claude Code, Codex, Grok u opencode) corriendo en una terminal de
verdad dentro de un panel del lienzo.

## Qué corre ahí dentro

- **El programa entero**: los comandos de barra, el selector de modelo, los diffs y las peticiones de
  permiso son los de la propia CLI, y escribes en ellos como escribirías en la Terminal.
- **La configuración que ya está en el proyecto**: las instrucciones escritas en la carpeta, los
  servidores MCP y los subagentes los lee la CLI, que corre en la carpeta del lienzo.
- **El binario instalado en esta máquina**: la app busca cada CLI en tu `PATH` y muestra en
  **Ajustes → Proveedores** cuáles encontró. Ver [varios proveedores](varios-provedores).

## La carpeta

El directorio de trabajo no se elige al crear el agente: viene del lienzo, y todo agente creado ahí
nace en él. Ver [elegir el proyecto](escolher-o-projeto).

## El nombre

El nombre se elige al crear el agente, con una sugerencia ya escrita, y es por él que lo llamas por
voz, en el `⌘K` y en el panel de elenco.

- **Mientras el agente exista en el proyecto**, en pantalla o guardado, su nombre queda reservado y
  ningún agente nuevo puede recibirlo.
- **Olvidar a un agente devuelve el nombre** al conjunto de nombres disponibles. Ver
  [crear y cerrar](criar-e-fechar).

## Permisos

En los ajustes del lienzo está el interruptor **No pedir permiso**, activado por defecto.
Desactivado, la CLI vuelve a pedir permiso antes de cada herramienta, el agente queda en estado de
espera mientras la petición no se responda, y la app te avisa. El menú de modo de permiso solo
aparece con el interruptor desactivado. Ver [ajustes del proyecto](ajustes-projeto).

## Su propio navegador

Un agente puede abrir un navegador en el lienzo, y ese panel es suyo: ningún otro agente navega, hace
clic ni toma una captura ahí. Ver [el agente ve el navegador](o-agente-ve-o-navegador).

## El panel y el agente son cosas distintas

Cerrar el panel despide al agente y guarda la conversación, el nombre, la última tarea y lo que él
registró como entregado. Ver [crear y cerrar](criar-e-fechar).
