---
slug: skills-e-mcp
titulo: Skills y servidores MCP
resumo: Qué le dan una skill y un servidor MCP a los agentes de este proyecto, y qué se le puede pedir a un agente sin abrir ninguna pantalla.
area: agentes
nivel: avancado
---

Una **skill** es un archivo de instrucciones que el agente carga cuando aparece su tema. Un
**servidor MCP** es un programa que entrega herramientas al agente, como una base de datos, un issue
tracker o un servicio de la empresa.

Las dos cosas se gestionan por las pantallas ([skills](ajustes-skills), [MCP](ajustes-mcp)) o
pidiéndoselo a un agente. Los dos caminos tocan el mismo acervo.

## Qué hace un agente con las skills

- **Listar**: devuelve las skills que este proyecto tiene a mano, con el nombre, la descripción, los
  programas de agente que la ven y si está activa en este canvas.
- **Buscar**: consulta un registro público por tema, tecnología o nombre, y devuelve los candidatos
  con descripción, estrellas y el repositorio de origen. Buscar no instala nada. Si el registro no
  está disponible, el agente avisa.
- **Instalar**: descarga la skill del repositorio de origen, en el proyecto o en tu cuenta. El valor
  predeterminado es el proyecto. Pedida por voz, la instalación va siempre al proyecto.
- **Escribir**: el agente redacta el archivo entero de la skill, encabezado incluido. Por aquí pasan
  "mejora esta skill" y "junta estas tres en una". Una skill con
  el mismo nombre en el mismo lugar se sobrescribe, y el nombre pasa a ser el de la carpeta.
- **Activar y desactivar**: vale solo en este canvas y solo para los agentes iniciados a partir de
  ahí. Nada sale del disco.
- **Eliminar**: borra la skill del disco, sin deshacer. Las skills nativas del programa de agente no
  se pueden eliminar.

## Qué hace un agente con los servidores MCP

- **Listar**: devuelve los servidores que instaló CanvasCode, con el estado de cada uno en este
  canvas, y los que configuraste por fuera.
- **Buscar**: consulta el registro oficial, que es público y no pide cuenta. El resultado dice el
  nombre exacto, si el servidor habla por HTTP o levanta un proceso, y si pide clave.
- **Instalar**: instala desde el registro y deja el servidor activo solo en este canvas. Las claves
  que pida van al Keychain del Mac; las que falten quedan para que las completes en la pantalla de
  MCP.
- **Activar y desactivar**: vale para los agentes iniciados a partir de entonces. Los que ya están en
  pie siguen con los servidores con los que nacieron hasta que renazcan.

## Dónde vive una skill

- **En este proyecto**: dentro del repositorio, versionada con el código, y por lo tanto disponible
  para quien clone el proyecto.
- **En tu cuenta**: vale en todos tus proyectos.
- **Nativa del programa de agente**: viene con él, y CanvasCode no la elimina.

Al instalar o escribir una skill, eliges entre las dos primeras.

## Desactivar no es eliminar

Desactivar pide a los agentes de este proyecto que no usen esa skill, y se deshace con un clic.
Eliminar borra el archivo del disco y no tiene vuelta. Para dejar de usar una skill solo aquí,
desactívala.

## Lo que cuesta cada servidor

- **HTTP**: el servidor es compartido y no cuesta ningún proceso por agente.
- **Proceso**: levanta un proceso por agente, unos 60 MB cada uno. Con seis agentes en pantalla, son
  seis procesos de ese servidor.

El servidor MCP del propio CanvasCode queda fuera de esa cuenta: es uno solo, dentro de la app,
compartido por todos los agentes.

## Instalar es dejar correr código de terceros

Una skill trae instrucciones escritas por otra persona, y un servidor MCP trae código que pasa a
correr junto a tus agentes. El agente confirma el origen contigo antes de instalar, y un servidor
instalado desde aquí nace activo solo en el canvas desde el que partió la instalación.

## Configurado en otra pantalla

- La lista de skills de este proyecto: [Ajustes · Skills](ajustes-skills).
- La lista de servidores MCP: [Ajustes · MCP](ajustes-mcp).
