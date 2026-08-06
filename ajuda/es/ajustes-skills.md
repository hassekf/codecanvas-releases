---
slug: ajustes-skills
titulo: Ajustes · Skills
resumo: La pantalla que lista las skills que este proyecto tiene a mano, activa y desactiva cada una aquí, e instala desde el registro público.
area: projeto
nivel: avancado
---

En **Editar el proyecto → Skills**. La pestaña solo existe en un proyecto ya creado.

## La lista

Las skills vienen agrupadas por origen, y cada fila trae el nombre, la descripción y una etiqueta por
cada programa de agente que la ve.

- **En este proyecto**: están en el repositorio y se versionan con el código.
- **Global del proveedor**: están en tu cuenta y valen en todos tus proyectos.
- **Del sistema**: nativas del programa de agente. Llevan un candado, se abren en solo lectura y no
  se pueden eliminar.
- **Sin ningún programa de agente instalado en la máquina**, la pestaña lo dice y no lista nada: no
  hay de dónde descubrir skills.

## El interruptor de cada fila

- **Desactivar** pide a los agentes de este proyecto que no usen esa skill, y vale para los agentes
  iniciados a partir de ahí. Quien ya está en pie sigue como nació.
- **La skill desactivada sigue en la lista**, atenuada, y nada sale del disco.
- **El efecto es solo de este canvas.** La misma skill sigue valiendo en tus otros proyectos.

## El menú de cada fila

- **Ver / editar SKILL.md**: abre el archivo de la skill para leerlo y editarlo. En las del sistema,
  solo lectura.
- **Eliminar…**: borra la skill del disco, incluidos los accesos que la compartían entre programas de
  agente. Pide confirmación y no tiene deshacer. Para dejar de usarla solo aquí, usa el interruptor.

## Instalar

**Instalar skills…**, arriba en la pestaña, abre la búsqueda en el registro público.

- **El campo de búsqueda** filtra por tema, tecnología o nombre, y cada resultado trae descripción,
  estrellas y el repositorio de origen.
- **Elegir un resultado** abre la confirmación, con el enlace al repositorio. Es código de terceros,
  y el origen se comprueba ahí mismo.
- **Dónde instalar**: **En este proyecto**, versionada en el repositorio, o **En mi cuenta**, válida
  en todos tus proyectos.
- **Con el registro no disponible**, la ventana lo dice en lugar de seguir buscando.
- **La instalación falla** cuando el repositorio es privado, no está disponible, o no tiene el
  archivo de la skill en la ruta indicada. El motivo aparece en la propia ventana.

## Configurado en otra pantalla

- Qué es una skill, y qué se le puede pedir a un agente: [skills y servidores MCP](skills-e-mcp).
- Los servidores de herramientas de este proyecto: [Ajustes · MCP](ajustes-mcp).
