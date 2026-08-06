---
slug: painel-webcam-e-avatar
titulo: La cámara y el avatar
resumo: El panel con la imagen de tu cámara y el panel con el rostro de la asistente: dónde están los controles, cuándo se apaga la cámara sola, y qué cambia al soltar el panel de la cuadrícula.
area: paineis
nivel: basico
---

Los dos se abren con `⌘K` (escribe "webcam" o "avatar").

## El panel de webcam

El cuerpo del panel es solo la imagen. Los controles están en el menú del clic derecho, que se abre
tanto sobre la cabecera como sobre la imagen:

- **Cámara**: elige la fuente de la imagen. La lista trae las cámaras que macOS ve en ese momento,
  incluidas la Continuity Camera y la Desk View del iPhone. **Predeterminada del sistema** deja la
  elección a macOS. Conectar o desconectar una cámara actualiza la lista sin reabrir el panel.
- **Reflejar la imagen**: invierte la imagen en horizontal. La captura no se reinicia.

La cámara y el reflejo elegidos quedan guardados en el panel, y al reabrir la app vuelven. Si la
cámara elegida desaparece, el panel vuelve solo a la predeterminada del sistema en vez de quedarse
sin imagen.

### Un solo panel en toda la app

Existe **un** panel de webcam, no uno por proyecto. Abrir la webcam en un lienzo donde no está lleva
el panel allí, y la captura no se interrumpe en el cambio.

### Cuándo se apaga la cámara sola

- **Durante una reunión**: el panel libera la cámara para la llamada y la retoma cuando la reunión
  termina. Ver [agenda y reuniones](agenda-e-reunioes).
- **Con la ventana de la app cerrada**: la app sigue funcionando sin la ventana, y la cámara se
  libera junto con ella.

La cámara solo vuelve a capturar cuando ninguna de esas razones está activa.

### Fuera de la cuadrícula, queda la imagen

Con el lienzo en disposición automática, la cabecera tiene el botón **Soltar da grade**. Fuera de la
cuadrícula y sin selección, el panel de webcam pierde la cabecera y el borde: queda solo la imagen.
En ese estado se mueve arrastrando la propia imagen, y un clic devuelve los controles.

### El permiso

macOS pide el acceso a la cámara la primera vez. Denegado el acceso, el panel muestra **El acceso a
la cámara está bloqueado** y la ruta para permitirlo en Ajustes del Sistema. Autorizado, pero sin
ninguna cámara disponible, muestra **No se encontró ninguna cámara**. Ver
[los permisos que pide macOS](permissoes-do-mac).

### Por voz

Abrir el panel, reflejar, quitar el reflejo y cambiar de cámara diciendo un trozo de su nombre ("usa
la del iPhone"). Con el panel cerrado, el comando lo abre antes de hacer el resto.

## Con qué cámara nace un panel nuevo

En **Configuración → Webcam**.

- **Cámara predeterminada**: la cámara con la que abre un panel de webcam nuevo.
- **Reflejar la imagen de forma predeterminada**: si un panel nuevo nace con la imagen invertida.

Los dos valen para el **próximo** panel. Ninguno cambia el panel ya abierto, que guarda la elección
hecha en él.

## El panel del avatar

El rostro de la asistente, dibujado en caracteres sobre un fondo animado. El dibujo corre en una
página local dentro de la app: nada de él sale de tu máquina.

El panel no tiene ningún control. Quien lo mueve es la conversación por voz:

- al **abrir la conversación**, el rostro se condensa desde el fondo;
- mientras **ella habla**, la boca sigue el nivel de la voz que sale;
- al **cerrar la conversación**, el rostro se disuelve y queda el fondo.

El rostro adopta el color de acento del tema del lienzo en el que está el panel, y cambia junto
cuando cambias de proyecto. Ver [apariencia](aparencia).

Como la webcam, el avatar es **uno solo en toda la app** y queda sin cabecera ni borde cuando está
fuera de la cuadrícula.

Para lo que la asistente hace además de aparecer, ver [hablar con Nina](falar-com-a-nina).
