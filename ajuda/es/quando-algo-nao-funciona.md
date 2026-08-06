---
slug: quando-algo-nao-funciona
titulo: Cuando algo no funciona
resumo: Síntoma y acción: qué hacer ante cada fallo común de CanvasCode, y dónde la app ya muestra la causa.
area: conta
nivel: basico
---

## El panel del agente no abre ningún terminal

El panel dice cuál es el caso.

- **"Claude Code no está instalado."**: haz clic en **Instalar ahora**. La instalación es local y no
  pide contraseña de administrador. Mira [el primer agente](primeiro-agente).
- **Otro CLI declarado como no instalado**: el panel muestra su comando de instalación. Ejecuta el
  comando en un terminal y reabre la app. Mira [varios proveedores](varios-provedores).
- **"Preparando el agente…"**: la app le está preguntando a la shell dónde vive el CLI. Espera unos
  segundos.

## Un agente se detuvo a mitad y parece que terminó

Es el proveedor tumbando al agente. La app avisa con una notificación que no desaparece sola y, con
la recuperación automática activada, le manda al agente continuar, espaciando cada nuevo intento. No
insiste ante una credencial rechazada, un servicio caído o una conversación demasiado llena.

- **Para activar o desactivar la recuperación**: **Reanudar agentes que la API tumbe**, en
  [configuración de los agentes](ajustes-agentes). Desactivada, el fallo se sigue mostrando y
  anunciando, y tú retomas con el botón del aviso, por voz, o escribiendo en el terminal del agente.
- **Para saber si esto pasa demasiado**: **Ajustes → Diagnóstico**, en **Fallos por error de API**.
  Son los últimos siete días, por proveedor, con cuántos se reanudaron solos y un gráfico por día.
  **Limpiar registro** pone la cuenta a cero.

## No sé si el problema es mío o del proveedor

En el pie, el sello de cada proveedor muestra el estado de su servicio. Pasa el ratón para leer el
mensaje, y haz clic para abrir la página de estado en un panel de navegador.

## Un agente volvió sin recordar nada

La conversación de un agente vive dentro de la cuenta en la que nació. La app avisa en qué cuenta
buscó y, cuando la conversación está en otra cuenta registrada, dice cuál es.

**Cambia la cuenta de ese agente** para traer la conversación: clic derecho en su panel y elige en
el menú de cuenta. La app no mueve la conversación sola. Mira
[cuentas y perfiles](contas-e-perfis).

## Un agente dice que no tiene permiso para leer un archivo

macOS le exige a CanvasCode el permiso de acceso a Documentos, Escritorio y Descargas, y el agente
recibe solo un error de acceso denegado.

Concédelo en **Ajustes del Sistema → Privacidad y seguridad → Archivos y carpetas**. Mira
[los permisos que pide macOS](permissoes-do-mac).

## Nina no te oye

1. Abre **Ajustes → Diagnóstico** y lee el estado del **Micrófono**. Está escrito en portugués:
   `liberado` (concedido), `negado` (denegado), `bloqueado` (restringido) o `nunca perguntado`
   (nunca preguntado).
2. En `nunca perguntado`, haz clic en **Pedir permiso**.
3. En `negado` o `bloqueado`, haz clic en **Borrar los permisos y preguntar de nuevo**. macOS no
   pregunta dos veces, y este botón borra el registro de permiso de esta app para que vuelva a
   preguntar desde cero. La app se reabre después, y no se borra nada más.
4. Estando `liberado`, revisa el **Micrófono** en **Ajustes → Voz** y usa **Probar el micrófono**,
   justo debajo. Un medidor parado en cero suele ser macOS captando de otro dispositivo.

Si deja de oírte en medio de una conversación que funcionaba, el indicador de voz muestra
"reconectando…" y la conexión vuelve sola. Más en [configurar la voz](configurar-a-voz).

## Las pestañas de Issues y PRs están vacías

Dependen de `gh`, la herramienta de línea de comandos de GitHub. La propia pestaña dice cuál es el
caso: `gh` no instalado, `gh` sin sesión iniciada (`gh auth login`), o el proyecto sin un remoto de
GitHub. Mira [el panel de Git](painel-git).

## La app no abre

Después de fallar dos veces seguidas al arrancar, la app sube en una pantalla de recuperación, sin
cargar los proyectos ni los agentes, ofreciendo las copias.

Elige un punto de la lista y haz clic en **Restaurar todo**, **Solo las configuraciones** (cuando
fue una preferencia la que rompió la app) o **Solo los proyectos**. El estado actual se guarda antes
de restaurar. Sin ninguna copia en la lista, queda abrir de todos modos, y la app intenta empezar de
cero.

La misma pantalla está en **Ajustes → Copias**, en **Restaurar desde una copia…**, junto a **Hacer
copia ahora** y la frecuencia de las copias.

## Algo quedó raro después de tocar los ajustes

**Restaurar predeterminados**, al pie de la barra lateral de los Ajustes. Pide confirmación y
devuelve al original la fuente, la escala, el ancho máximo, los atajos, la voz y los paneles de
subagente, además de desanclar la versión de Claude Code. No se ven afectados: tu clave de OpenAI,
los dispositivos de audio y los temas de los lienzos.

## El instalador aparece como dañado

La descarga vino incompleta. Descárgalo de nuevo. Mira [instalar](instalar).

## Reportar un problema

- **El número de versión** está al pie de la barra lateral de los Ajustes.
- **El diario de la voz** registra cada conexión, caída y reconexión. Los botones **Mostrar en el
  Finder** y **Abrir** están en **Ajustes → Diagnóstico**, y siempre graba.
- **Los informes de fallo** de macOS se pueden enviar con el interruptor **Enviar informes de fallo
  y de reanudación fallida**, en el mismo lugar. La lista de los fallos registrados queda justo
  debajo, con un botón **Enviar** en cada uno. Mira
  [dónde están mis datos](onde-ficam-meus-dados).
