---
slug: permissoes-do-mac
titulo: Los permisos que pide macOS
resumo: Cada permiso que pregunta el sistema, qué desbloquea, qué se rompe al negarlo, y cómo hacer que el Mac pregunte de nuevo.
area: comecando
nivel: basico
---

macOS pregunta la primera vez que usas cada función. Ninguno se pide al arrancar.

## Los permisos

- **Micrófono**: sin él, la conversación por voz y el dictado no funcionan. Ver
  [configurar la voz](configurar-a-voz).
- **Reconocimiento de voz**: lo usa el dictado que corre en tu propio Mac. Ver [dictado](ditado).
- **Grabación de pantalla**: sin ella, grabar la ventana de la app no funciona. Ver
  [el panel de grabación](painel-gravacao).
- **Cámara**: la imagen aparece en [el panel de cámara](painel-webcam-e-avatar) y no sale de tu Mac.
- **Calendario**: la app lee tu agenda para avisar de las reuniones y abrir el enlace de la llamada.
  No se escribe nada en tu calendario. Ver [agenda y reuniones](agenda-e-reunioes).
- **Notificaciones**: los avisos de macOS con la app en segundo plano. El permiso solo se pide
  después de que actives "Avisar en el Mac fuera de la app" en [avisos y sonidos](avisos-e-sons).
- **Escritorio, Documentos y Descargas**: las carpetas en las que los agentes leen y escriben.

## El acceso a las carpetas

**macOS le cobra el permiso a CanvasCode, no al programa del agente.** Un agente abierto aquí dentro
es un proceso hijo, y el sistema atribuye el acceso al responsable.

Negarlo no produce una petición de permiso en la terminal del agente. Él recibe un error seco de
acceso denegado, y con frecuencia concluye que el archivo no existe.

Para habilitarlo después: Ajustes del Sistema → Privacidad y Seguridad → Archivos y Carpetas, y
habilita CanvasCode para la carpeta en cuestión.

## Cuando macOS dejó de preguntar

Un permiso negado no se vuelve a preguntar: la petición responde "no" al momento, sin diálogo. Esto
pasa también cuando existe un registro antiguo de esta app hecho por un binario con otra firma, como
una compilación de desarrollo o una versión anterior.

En **Configuración → Diagnóstico** están:

- el estado de **Micrófono**, **Reconocimiento de voz** y **Grabación de pantalla**;
- **Pedir permiso**, que solo tiene efecto mientras el sistema aún no ha decidido;
- **Abrir Ajustes del Sistema** y **Grabación de Pantalla en Ajustes**, que llevan a cada panel del
  sistema;
- **Volver a comprobar**, que relee el estado;
- **Borrar los permisos y preguntar de nuevo**, que aparece cuando alguno está negado. Borra el
  registro de permiso de esta app, y de nada más. **La app tiene que reabrirse después**, y las
  preguntas vuelven a empezar.
