---
slug: ajustes-integracoes
titulo: Integraciones
resumo: La agenda del Mac en Configuración, qué ve Nina de ella, y por qué Jira se conecta en la edición del proyecto.
area: ajustes
nivel: basico
---

En **Configuración → Integraciones**.

## La agenda del Mac

- **Conectar la agenda**: trae los compromisos de todas las cuentas que tu Mac ya tiene, incluidas
  iCloud, Google y Exchange. La app solo lee la agenda; nunca escribe nada en ella. Al encenderla,
  macOS pide el permiso. Si lo niegas, el interruptor vuelve a apagado.
- **macOS negó el acceso**: aparece debajo del interruptor cuando el permiso fue negado. macOS no
  vuelve a preguntar solo, y **Abrir Ajustes del Sistema** lleva a la pantalla de Calendarios. Los
  demás permisos están en [los permisos que pide macOS](permissoes-do-mac).

Apagada, la agenda no existe para la app: nada en la pantalla inicial, ningún aviso, y Nina no recibe
la herramienta de agenda.

Encendida, aparecen los controles de abajo.

- **Lo que Nina puede ver**: cinco interruptores, uno por dato del compromiso (el título, el lugar, la
  descripción y el orden del día, los participantes y el enlace de la llamada). Solo lo que esté
  encendido sube a OpenAI, y solo cuando le preguntas a Nina sobre la agenda. Los compromisos que se
  muestran en la pantalla de la app no salen de tu Mac. El enlace de la llamada es lo que ella
  necesita para abrir la reunión por voz.
- **Qué agendas entran**: un interruptor por calendario que el Mac tiene, con la cuenta de cada uno.
  Ninguno marcado quiere decir todos; la primera desmarcación materializa la lista.
- **Avisar antes de la reunión**: el aviso aparece antes del comienzo y se queda hasta que entres o lo
  descartes.
- **Avisar antes**: 5, 10, 15 o 30 minutos antes. Solo aparece con el aviso encendido.
- **Al abrir una reunión**: **En un panel de aquí**, que abre la llamada en un navegador del lienzo ya
  con tu sesión de Google iniciada, o **En mi navegador**. Puedes cambiarlo en el momento, en el
  propio aviso.

Lo que pasa el día de la reunión está en [agenda y reuniones](agenda-e-reunioes).

## Atlassian

Jira y Confluence no se conectan aquí: la conexión es de cada lienzo.

- **Jira de "<nombre del proyecto>"**: con un proyecto abierto, el botón **Conectar** o **Editar** abre
  la edición de ese workspace ya en la parte de Atlassian. El texto de al lado dice si ya está
  conectado.
- **Ningún workspace abierto**: sin proyecto abierto no hay qué conectar, y la pantalla lo dice.

El paso a paso está en [Jira y Confluence](jira-e-confluence).

## Dónde viven los secretos

Toda credencial de integración se guarda en el Keychain de tu Mac, nunca en un archivo de la app, y
desconectar borra la credencial junto.
