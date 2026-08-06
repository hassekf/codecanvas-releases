---
slug: primeiro-agente
titulo: El primer agente
resumo: Instalar el programa de agente, crear el panel, mandar la primera tarea y leer su estado.
area: comecando
nivel: basico
---

Un agente es el programa de línea de comandos corriendo dentro de un panel, con la terminal entera
funcionando.

## Instalar el programa de agente

Si Claude Code no está en la máquina, el panel del agente nuevo muestra **Instalar ahora**. La
instalación es local y no pide contraseña de administrador.

Mientras el panel dice **Preparando el agente…**, la app está averiguando dónde vive el programa.
Tarda unos segundos.

Otros programas de agente corren en el mismo lienzo: Codex, Grok y opencode. Cada uno se activa en
Configuración → Proveedores. Ver [varios proveedores](varios-provedores).

## Crear

- `⌘N`. Funciona incluso con el cursor dentro de otro agente, y el panel nuevo nace con el cursor
  dentro de él.
- `⌘⇧N` crea un agente de Codex, y la tecla solo hace algo con Codex activado en la Configuración.
- `⌘K`, y escribe **agente**.
- El botón de agente nuevo, en la barra del lienzo.
- Con la voz configurada, `⌥C` y *"abre un agente"*.

`⌘T` abre una terminal en el mismo sitio, sin ningún agente encima. Ver
[el panel de terminal](painel-terminal).

## El nombre

Cada agente nace con un nombre propio. Por él lo llaman la voz, el `⌘K` y los demás agentes, y es el
nombre que aparece en [el elenco](painel-elenco) después de descartarlo.

## La primera tarea

Escribe en el panel como escribirías en tu propia terminal. *"Explícame qué hace este proyecto"* es
una petición corta y comprobable: lee los archivos, responde, y ves el panel cambiar de estado por el
camino.

## El estado del panel

El indicador de cada panel tiene cinco estados: **parado**, **trabajando**, **esperándote**,
**caído** y **cerrado**.

**Caído** es el turno terminado por un error; **parado** es el turno completado. La recuperación
automática del agente caído se configura en [configuración de los agentes](ajustes-agentes).

`⌥F` voltea todos los paneles a la vez y muestra el resumen de cada agente: la misión, qué hizo y
hace cuánto. Ver [saber qué están haciendo](saber-o-que-fazem).

## Cuando no abre

El panel dice qué falta: el programa de agente sin instalar, o la app aún buscando dónde vive. Para
lo demás, ver [cuando algo no funciona](quando-algo-nao-funciona).
