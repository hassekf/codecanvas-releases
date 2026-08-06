---
slug: avisos-e-sons
titulo: Avisos y sonidos
resumo: Notificaciones de CanvasCode en el lienzo y en macOS: qué eventos avisan, sonido y lectura en voz alta.
area: ajustes
nivel: basico
---

En **Configuración → Notificaciones**.

## Dentro de la app

Notificaciones mostradas en el lienzo, con CanvasCode en primer plano.

- **Un agente terminó**: notifica cuando el agente completa la tarea.
- **Un agente te está esperando**: notifica cuando el agente hace una pregunta o pide un permiso.
- **Un agente se cayó**: notifica cuando el agente se interrumpe por un error. Desactivarlo suprime
  la notificación y no afecta la recuperación automática, configurada en
  [configuración de los agentes](ajustes-agentes).
- **Se acerca el plazo de una tarea**: notifica 1 hora antes del vencimiento, 30 minutos antes y al
  vencer. Los plazos vienen del [panel de tareas](painel-tarefas), y este es el único evento sin
  equivalente en la sección siguiente.

Cada uno de los cuatro tiene dos opciones:

- **Reproducir sonido**: emite un toque corto junto con la notificación.
- **Leer en voz alta**: la app lee el aviso, solo con el panel del agente fuera de vista, incluido el
  caso de estar en otra área de trabajo. No disponible mientras la voz no esté configurada en
  [configurar la voz](configurar-a-voz).

## Fuera de la app

Notificaciones de macOS, emitidas solo con CanvasCode en segundo plano.

- **Avisar en el Mac fuera de la app**: habilita las notificaciones del sistema. Desactivado, los
  controles de abajo quedan no disponibles y la app no solicita el permiso de notificación a macOS.
  Si las notificaciones no aparecen tras activarlo, revisa el permiso en
  [los permisos que pide macOS](permissoes-do-mac).
- **Un agente terminó**, **Un agente te está esperando** y **Un agente se cayó**: notifican los
  mismos eventos de la sección anterior, por macOS. Cada uno tiene la opción **Reproducir sonido**.

## El sonido de los avisos

- **Reproducir sonido en los avisos**: activa y desactiva el sonido de todas las notificaciones, de
  las dos secciones anteriores. Desactivado, ninguna notificación emite sonido y las opciones
  **Reproducir sonido** quedan no disponibles.

## Modo reunión

Durante el [modo reunión](agenda-e-reunioes) no se muestra ni se lee ninguna notificación.

## Configurado en otra pantalla

- La voz que lee los avisos: [configurar la voz](configurar-a-voz).
- El brillo del panel al completar una tarea: [saber qué están haciendo](saber-o-que-fazem).
- Los anuncios emitidos por los agentes: [anuncios](ajustes-anuncios).
