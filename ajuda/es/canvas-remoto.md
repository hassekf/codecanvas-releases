---
slug: canvas-remoto
titulo: El canvas en un servidor
resumo: Cómo apuntar un proyecto a otra máquina, qué comprueba la prueba de conexión, qué pasa cuando se cae la red y qué todavía no funciona a distancia.
area: integracoes
nivel: avancado
---

Un canvas puede vivir en otra máquina. Los agentes nacen y trabajan allí, y este Mac es la vista. La
app llega al servidor por SSH, y no instala ni deja nada escuchando del otro lado.

Esta parte de CanvasCode está en construcción. Lo que todavía no funciona está al final de la página.

## Elegir la máquina

En **Editar el proyecto → Proyecto → Dónde vive este proyecto**.

- **En esta máquina** y **En un servidor mío**: deciden dónde trabajan los agentes de este canvas.
  Elegir el servidor oculta el campo de la carpeta local.
- **El menú de servidores** lista los registrados y trae **Añadir servidor…**. Un servidor registrado
  pertenece a la app, no al canvas: la misma máquina sirve a varios proyectos.
- **Cambiar de servidor limpia la carpeta elegida**.
- **Editar…**: vuelve a abrir el registro de ese servidor.

## Registrar un servidor

- **Apodo**: cómo aparece ese servidor en la lista y cómo lo llama la voz.
- **Dirección**: la IP o el dominio, el usuario y el puerto del SSH.
- **Clave**: la ruta de la clave privada. En blanco, la app usa la clave con la que ya entras en esa
  máquina.
- **Probar conexión**: dice si alcanzó la máquina, cuál es el sistema, y si están ahí git, tmux, node
  y el programa de agente. Cuando el programa de agente está instalado pero sin credencial, la prueba
  avisa: sin eso el agente arranca, se queda callado y parece trabado.
- **Guardar** queda no disponible mientras la dirección esté vacía.

## Elegir la carpeta

**Elegir carpeta…** abre un navegador por las carpetas del servidor.

- **Arriba** sube un nivel, y **Nueva carpeta…** crea una carpeta ahí.
- **Las carpetas que son repositorio** vienen marcadas.
- **Usar esta carpeta** cierra el navegador con la elección. La app prepara el resto sola.

## Lo que funciona igual

- **La terminal de cada agente**, con su pantalla entera.
- **El estado del agente**: la luz del panel, el asunto, quién escribió en cada archivo, la pregunta
  pendiente.
- **El Git del repositorio de allá**, en el panel de siempre.
- **El cajón de archivos**, y abrir un archivo en un panel para leerlo.
- **Arrastrar un archivo hasta un agente**: el archivo sube primero al servidor, y el agente recibe
  la ruta de allá. Si el envío falla, no se pega nada en el prompt y la app dice el motivo.

## Cuando se cae la red

El SSH de un agente que muere no es el agente muriendo: la sesión sigue viva del otro lado.

- **El aviso aparece en la pantalla del propio panel**, diciendo qué conexión se cayó y en cuántos
  segundos la app lo intenta de nuevo.
- **La espera crece en cada intento**, de 3 segundos hasta el tope de 30.
- **Al reconectar, la sesión se reencuentra** con el historial y la pregunta pendiente donde estaban.
- **Un panel cerrado no reconecta.** El agente sigue vivo en el servidor, y lo traes de vuelta como a
  cualquier agente guardado.

## Si entras como root

El programa de agente se niega a correr como root con los permisos liberados. En ese caso la app
quita esa opción: el agente arranca y vuelve a pedir permiso antes de cada herramienta, y la app
trata esos pedidos como siempre. La prueba de conexión avisa cuando el usuario es root.

## Lo que todavía no funciona

- **Editar un archivo remoto**: el panel abre y muestra el contenido, y el botón de editar no
  aparece.
- **Seguir un archivo remoto en vivo**: no se vigila como el de aquí, y se relee cuando lo pides.
- **El navegador del agente es un panel de este Mac.** Sin el Mac encendido, el agente remoto se
  queda sin ver la página que produjo.
- **Los módulos los sirve la app**, y por lo tanto solo existen con el Mac encendido.
- **Los paneles de Uso y de Rendimiento** miden esta máquina.
- **Dos Macs en el mismo canvas** todavía no se combinan.

## Configurado en otra pantalla

- La carpeta de un proyecto local: [ajustes del proyecto](ajustes-projeto).
- Cambiar de proyecto: [elegir el proyecto](escolher-o-projeto).
