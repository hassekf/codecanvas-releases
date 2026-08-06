---
slug: ajustes-agentes
titulo: Configuración de los agentes
resumo: La pestaña Agentes, control por control, y los tres ajustes de agente que viven en la pestaña Interfaz.
area: ajustes
nivel: basico
---

En **Ajustes → Agentes**. Lo que está aquí vale para todos los proyectos. Lo que es de un solo
proyecto (la cuenta en que nacen sus agentes, el modelo, los permisos, el navegador predeterminado)
está en los ajustes del lienzo. Ver [ajustes del proyecto](ajustes-projeto).

- **Historial de entregas del agente**: activado, cada asunto concluido se vuelve una línea en el
  reverso del panel cuando el agente pasa al asunto siguiente. Desactivado, el reverso muestra solo
  lo que hace ahora.
- **Reanudar agentes que la API tumbe**: activado, la app le manda al agente continuar desde donde
  quedó tras una caída de la API, esperando más en cada nuevo intento. El aviso de la caída ocurre
  con él activado o desactivado. Ver [crear y cerrar](criar-e-fechar).
- **Hibernar agentes inactivos**: desactivado por defecto. Activado, el agente sin actividad por el
  tiempo de abajo se cierra, el panel queda con un botón de despertar y la conversación se reanuda
  cuando el agente vuelve.
  - **Dormir después de**: aparece dentro del control de arriba, y solo con él activado. Va de 5
    minutos a 8 horas, y viene en 1 hora. El reloj se reinicia con cada herramienta usada, con cada
    prompt enviado y siempre que abres el panel del agente. Nunca duermen quien está trabajando,
    quien espera tu respuesta y el panel seleccionado en el lienzo en foco.
- **Instalaciones de Claude**: registra carpetas `.claude`, cada una con su propio inicio de sesión,
  servidores y conversaciones. **Agregar instalación…** pide la carpeta. Quitar una de la lista no
  borra nada del disco, y la app pregunta qué hacer con los agentes que dependían de ella. Ver
  [cuentas y perfiles](contas-e-perfis).
- **Versión de Claude Code**: **La más reciente** mantiene Claude Code actualizado solo al abrir la
  app, antes de que nazca ningún agente. El menú también lista las versiones presentes en la máquina,
  y fijar una desactiva la actualización automática. El cambio vale para los agentes creados de ahí
  en adelante.
- **Sello de pull request**: muestra el PR de cada agente en el panel, en el pie y en Git, con el
  estado de la integración continua. Desactivado, la app deja de consultarle a GitHub sobre tus PRs.
  Ver [el panel de Git](painel-git).
- **Dev servers en su propio panel**: desactivado por defecto. Activado, los comandos largos como un
  servidor de desarrollo o un observador de archivos se abren en un panel de terminal visible, en vez
  de correr dentro del agente. Ver [hablar con ellos](falar-com-eles).
- **Aislamiento por worktree**: activado, cada agente crea su propia copia del proyecto antes de
  escribir y hace commit en su rama. El texto del protocolo que reciben los agentes es editable justo
  abajo, y el editor solo aparece con el interruptor activado. Ver
  [worktrees y aislamiento](worktrees-e-isolamento).
- **Paneles de subagente**: **Mostrar subagentes en el canvas** le da un panel a cada tarea que un
  agente delega, hasta tres a la vez. Desactivado, los subagentes siguen trabajando sin aparecer. Ver
  [un agente llama a otro](um-agente-chama-outro).
- **Conversación entre proyectos**: cuántos mensajes libera una autorización tuya entre un agente de
  aquí y un agente de otro proyecto. Las opciones son 2, 4, 6, 10 y 20 mensajes, y el valor por
  defecto es 4. Agotados, necesitan una autorización nueva.

## En la pestaña Interfaz

- **Brillo en el panel al terminar**: el borde del panel brilla cuando el agente entrega, aunque no
  esté seleccionado.
- **Destacar la pestaña del área al terminar**: la pestaña del área parpadea cuando un agente
  termina, o pasa a esperarte, en un área que no estás viendo.
- **Color del destello de conclusión**: el color de los dos anteriores. El botón **Predeterminado**
  solo aparece después de que lo cambies, y lo devuelve.
- **Agrupar los agentes en pestañas**, en la sección **Barra de frentes**: en un área con más de un
  agente, comparten un solo panel, con el elegido a la vista y los demás en pestañas. Vale para las
  áreas nunca configuradas a mano; el menú contextual de cada área manda por encima. Ver
  [áreas de trabajo](areas-de-trabalho).
- **Ocultar las pestañas de área cuando esté anclada**, en la misma sección: las pestañas de arriba
  desaparecen y la barra de frentes pasa a listar las áreas, cambiar al hacer clic, crear, renombrar
  y parpadear. El control solo funciona con la barra anclada.
