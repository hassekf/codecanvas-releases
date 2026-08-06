---
slug: modulos-capacidades
titulo: Las capacidades de un módulo
resumo: El puente que la app inyecta en la página del módulo: red, scripts, contexto, tema, almacenamiento y notificaciones.
area: modulos
nivel: avancado
---

La app inyecta un objeto `painel` antes de cualquier script de la página. Todo devuelve una promesa, y
un error nativo se vuelve un rechazo.

- **`painel.fetch(url, opts)`**: una petición HTTP hecha por la app, sin restricción de origen.
  Devuelve estado, cuerpo y cabeceras.
- **`painel.executar(script, args)`**: ejecuta un ejecutable de su propia carpeta, con ella como
  directorio de trabajo; una ruta fuera de ella es rechazada. Devuelve el código de salida, la salida
  estándar y la de error, limitadas a 512 KB, con un tope de 120 segundos. El proceso recibe el
  workspace, el lienzo y el módulo en el entorno.
- **`painel.contexto()`**: el módulo, el lienzo y la carpeta del proyecto donde está este panel.
- **`painel.tema()`**: los colores de acento y la fuente del tema del lienzo, para que el panel no
  desentone.
- **`painel.guardar(chave, valor)`** y **`painel.ler(chave)`**: un almacenamiento pequeño, por módulo,
  compartido entre los lienzos. Quien quiera separarlo por proyecto incluye el workspace en la clave.
- **`painel.notificar(opcoes)`**: un aviso dentro de la app, con título y cuerpo. Las opciones deciden
  si es fijo o tiene duración, si suena, si se lee en voz alta, y si trae un botón que te lleva al
  panel o trae el panel hasta ti. Repetir el mismo `id` reescribe el aviso en su sitio en vez de
  apilar otro; **`painel.dispensarNotificacao(id)`** lo quita de la pantalla. Nunca va al Centro de
  Notificaciones de macOS.

Guarda tokens y contraseñas en un script de la carpeta, no en el HTML.

## Qué no hace la página

- **No navega**: el panel muestra el `index.html`, y un enlace hacia afuera se ignora. Imágenes, CSS y
  scripts remotos cargan con normalidad.
- **No hereda tus cookies**, ni las del panel de navegador ni las del panel de medios.

## La consola se captura

Lo que la página escribe en la consola, los errores de JavaScript y las promesas rechazadas llegan a
la app, y un agente lee todo eso junto con una foto del panel. Ese es el ciclo de quien está
escribiendo un módulo: editar, mirar la foto, leer el error, corregir.

No existe instalar un módulo de terceros: todo módulo se escribe en tu máquina, por ti o por tus
agentes.
