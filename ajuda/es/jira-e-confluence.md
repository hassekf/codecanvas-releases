---
slug: jira-e-confluence
titulo: Jira y Confluence
resumo: Conectar un proyecto a tu cuenta Atlassian, elegir el proyecto de Jira, encender los avisos y desconectar.
area: integracoes
nivel: basico
---

En la edición del proyecto, en **Integraciones → Atlassian**. Llegas ahí por el selector de proyecto,
a la izquierda de la barra de comando, en **Editar "<nombre>"…**, o por el acceso directo de
[Integraciones](ajustes-integracoes) en Configuración.

La conexión es de cada lienzo: la cuenta, el sitio y el token se quedan con ese proyecto, y ningún
otro lienzo los ve. El token se guarda en el Keychain de tu Mac, nunca en un archivo de la app.

## Conectar

- **Sitio**: la dirección de tu Atlassian, con el formato `empresa.atlassian.net`.
- **Correo**: el correo de tu cuenta.
- **Token de API**: generado en `id.atlassian.com`, en Seguridad → Tokens de API. Vale por sitio.
- **Traer Confluence también**: el mismo token, pero exponer la base de documentación es una elección
  aparte.
- **Conectar**: valida las credenciales. El campo del token se limpia después de conectar.

Conectado, la sección **Conectado** muestra el sitio y el nombre de la cuenta, y dice si Confluence
entró.

## El proyecto de Jira

- **Proyecto de Jira**: el menú lista los proyectos que alcanzan las credenciales. Ese proyecto es
  el que abre el panel y el que Nina asume cuando no dices cuál. **Ninguno** deshace la elección. Al
  lado de la etiqueta, la app muestra cuántas incidencias hay abiertas ahí.

Sin proyecto elegido, los avisos de abajo no están disponibles: no hay sobre qué preguntar.

## Los avisos de Jira

El Jira de la nube no le entrega tus notificaciones personales a una aplicación, así que quien
pregunta es la app, cada cierto tiempo, y solo sobre el proyecto de este lienzo. El aviso siempre es
escrito: una notificación en el lienzo y, con la app en segundo plano, una de macOS. Nunca hablado.

- **Avisarme de Jira**: el interruptor general de este proyecto. Apagado, la app no hace ninguna
  llamada. Nace apagado.
- **Te mencionaron**: alguien escribió tu nombre en un comentario. Es el único que trae la clave y el
  título de la tarjeta, y el único que ya viene encendido.
- **Te pasaron una tarjeta**: te volviste el responsable de una tarjeta que era de otra persona, o de
  nadie.
- **Crearon una tarjeta en el proyecto**: toda tarjeta nueva, tuya o no.
- **Preguntarle a Jira cada**: 5, 15, 30 o 60 minutos. El valor por defecto es 15, y menos de 5 no se
  ofrece.

El primer barrido de un proyecto no avisa nada: marca el instante y cuenta desde ahí. Después de un
tiempo con la app cerrada, la app mira como mucho las últimas 24 horas.

## Qué queda disponible después

- **El tablero en el lienzo**: las columnas de Jira, arrastrar para cambiar de estado, crear
  incidencias. Es el [panel de Jira](painel-jira).
- **Por voz**: *"¿qué hay en el tablero?"*, *"¿qué bugs están abiertos?"*, *"mueve la PROJ-12 a
  hecho"*.
- **Para los agentes de este lienzo**: leer el tablero, abrir una incidencia entera con sus
  comentarios, crear y mover.
- **Buscar en Confluence**: solo con el interruptor de Confluence encendido.

Las cuatro herramientas de voz forman el grupo **Jira e Confluence** en Configuración → Herramientas:
apagarlo mantiene la conexión de pie y saca Jira de las manos de Nina. En un lienzo desconectado ni
llegan a enviarse al modelo.

## Desconectar

- **Desconectar**: borra el token del Keychain y la conexión de ese lienzo. Las herramientas de voz
  desaparecen, los agentes pierden el acceso y el panel de Jira no tiene qué mostrar.
