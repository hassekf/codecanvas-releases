---
slug: escolher-o-projeto
titulo: Elegir el proyecto
resumo: Crear un proyecto, señalar la carpeta, cambiar de proyecto, y qué pasa con los agentes cuando la carpeta cambia.
area: comecando
nivel: basico
---

Un proyecto es una carpeta de tu disco. **Todo agente del proyecto nace dentro de ella**, y esa
carpeta es la que ven el Git, los archivos y el navegador de los agentes.

## Crear

En la pantalla inicial, **Nuevo proyecto**. La hoja tiene cinco pestañas, y solo la primera es
obligatoria:

- **Proyecto**: dónde vive el proyecto (en esta máquina o en un servidor tuyo), la carpeta y el
  nombre. Sin carpeta elegida, el botón **Crear** queda no disponible.
- **Agentes**: en qué instalación de Claude nacen los agentes de este proyecto, y las flags que se
  les pasan. Ver [configuración de los agentes](ajustes-agentes).
- **MCP**: los servidores que levantan los agentes de este proyecto. Ver
  [configuración de MCP](ajustes-mcp).
- **Navegador**: la página en la que abre un navegador nuevo aquí. Ver
  [configuración del navegador](ajustes-navegador).
- **Apariencia**: el tema, la fuente de la interfaz y el fondo. Ver [apariencia](aparencia).

Las pestañas de **Skills**, **Anuncios** e **Integraciones** solo existen después de crear el
proyecto: dependen de un proyecto real en el disco.

El proyecto puede vivir en otra máquina, con este Mac como vista. Ver
[lienzo remoto](canvas-remoto).

## Cambiar de proyecto

- `⌘1` a `⌘9` abren los proyectos por su posición. La tecla aparece en la esquina de cada tarjeta de
  la pantalla inicial. El modificador y el mapa se cambian en Configuración → Atajos.
- `⌘K` encuentra un proyecto por su nombre. Ver [búsqueda y comandos](busca-e-comandos).
- En la pantalla inicial, los proyectos aparecen como tarjetas, con la ruta de la carpeta, cuántos
  agentes están trabajando ahora y cuándo estuviste allí por última vez. El último abierto viene
  marcado.

Nada se pierde al cambiar: los paneles siguen donde estaban y los agentes siguen corriendo.

## Qué es de cada proyecto

- los lienzos, las áreas de trabajo y los paneles abiertos;
- los agentes, en pantalla y guardados;
- el tema, la fuente de la interfaz y el fondo. Ver [apariencia](aparencia);
- las skills y los servidores MCP activos;
- los anuncios;
- las integraciones. El Jira de un proyecto no aparece en otro. Ver
  [configuración de integraciones](ajustes-integracoes).

Un mismo proyecto puede tener varios lienzos. Ver [varios lienzos](varios-canvases).

## Cambiar la carpeta después

La carpeta se cambia en [configuración del proyecto](ajustes-projeto).

**La carpeta de un agente es la carpeta en la que nació su proceso**, y cambiar el campo no alcanza a
una terminal que ya está en pie. Con agentes corriendo, la app avisa antes de guardar y pregunta:

- **Reabrir con la conversación**: cada agente se cierra y se recrea en la carpeta nueva, llevando su
  conversación consigo. Vuelve recordándolo todo, y lo que estaba haciendo en ese instante se pierde.
- **Dejar en la carpeta antigua**: los procesos siguen vivos donde están, y solo los próximos agentes
  nacen en la carpeta nueva.

Cuando la conversación de algún agente no se pueda llevar, la app dice cuáles antes de tocar nada, y
tú decides si sigues.
