---
slug: falar-com-a-nina
titulo: Hablar con Nina
resumo: Abrir y cerrar la conversación por voz, qué cierra un turno, los dos relojes y el saludo.
area: nina
nivel: basico
---

**⌥C** abre y cierra la conversación por voz. Los ajustes están en **Ajustes → Conversación**, y el
saludo de la mañana, en **Ajustes → Saludo**.

Nina actúa en el lienzo con las mismas herramientas del [modo comando](o-modo-comando) y de
[la conversación escrita](a-nina-por-texto). Lo que puede hacer está en
[lo que ella puede hacer](o-que-ela-consegue-fazer); los grupos de herramientas se activan y
desactivan en Ajustes → Herramientas.

**El comando de voz entiende portugués.** La interfaz de la app habla español, portugués e inglés, y
el dictado sigue el idioma elegido, pero las órdenes habladas se interpretan en portugués.

## Abrir y cerrar

- **⌥C**: enciende y apaga la conversación. Es un interruptor, no un pulsar y hablar.
- **"Pode dormir"**, "tchau", "valeu", "chega": cierra la conversación. Ella no se despide; el
  silencio es la confirmación. Los agentes siguen trabajando.
- **Esc**: corta la conversación y el habla en curso, con la app en cualquier ventana.
- **Confirmar al activar**: hace que Nina diga una palabra cuando el micrófono se abre. Apagado, lo
  primero de la conversación es tu voz.
- **Palabra de apertura**: cambia esa palabra. En blanco, vale la palabra predeterminada del idioma
  activo.

Cuando la conversación se despierta por un aviso, no dice la palabra de apertura y ya entra sabiendo
de qué agente se trata.

La conversación por voz no guarda nada de una sesión a otra: una vez cerrada, la siguiente empieza sin
lo que se dijo antes. Quienes guardan memoria son los agentes, y
[la conversación escrita](a-nina-por-texto).

## Durante la conversación

- Empezar a hablar interrumpe a Nina en mitad de la frase.
- El turno se cierra por **silencio**, nunca por el largo de lo que dices. Cuánto silencio cuenta como
  final es **Silencio para que responda** (predeterminado 900 ms), y a partir de qué volumen el sonido
  cuenta como voz es **Sensibilidad del micrófono**, los dos en Ajustes → Conversación.
- El marco de la ventana se enciende mientras ella habla.
- Mientras la conversación está en marcha, el panel de medios queda silenciado.
- La conversación no se abre en [modo reunión](agenda-e-reunioes): ⌥C muestra una notificación
  diciendo que el micrófono está con la llamada, con el botón de salir al lado.

### Los dos relojes

- **Cerrar tras silencio**: cierra la conversación después de ese tiempo sin que nadie hable. De 0 a
  300 segundos, predeterminado 90. Cero lo desactiva.
- **Tiempo máximo de la conversación**: cierra al terminar el tiempo incluso mientras hablas, y es el
  único que garantiza un techo de gasto. De 0 a 30 minutos, predeterminado 5. Cero es sin techo. En el
  último minuto la ventanita de la voz muestra la cuenta atrás.

## Cuando la app habla primero

Un agente que termina, que pregunta o que se cae genera un aviso, y la app lo habla si hay alguna voz
activa. Qué eventos avisan, con sonido y con voz, está en [avisos y sonidos](avisos-e-sons).

- **Responder a los agentes por voz**: después del aviso hablado, la app abre el micrófono unos
  segundos para que respondas hablando. Apagado, solo avisa.
- **Ventana de respuesta**: cuánto dura esa escucha, de 0 a 15 segundos, predeterminado 6. Cero
  desactiva la escucha. Usa el reconocimiento local y no gasta créditos.

Lo que dices en esa ventana decide lo que pasa:

- **"Me leva lá"**, "abre o painel dele", el nombre del agente: te lleva hasta él, cambiando de
  proyecto y de área si hace falta.
- **"Depois"**, "beleza", "deixa pra lá": cierra la escucha sin hacer nada.
- **"Continua"**, "tenta de novo", "pode mandar": manda al agente retomar. Solo vale justo después de
  un aviso de caída.
- **"Só quando voltar ao ar"**: espera a que el proveedor vuelva antes de retomar. Solo vale justo
  después de un aviso de caída.
- **Cualquier otra frase**: despierta la conversación, sabiendo ya de qué agente hablaba el aviso.
  Basta una palabra que la app no reconozca para que la frase entera vaya a la conversación, y por eso
  una respuesta dirigida a un agente ("pode ir de Postgres") nunca se confunde con un comando de
  navegación.

Quedarte callado cierra la ventana sin gastar nada.

## El saludo de la mañana

En Ajustes → Saludo.

- **Buenos días al abrir**: la app te cuenta cómo está el día la primera vez que la abres en el día, y
  solo cuando hay algo pendiente. Con Nina activa, el saludo se vuelve conversación; con ella apagada
  y alguna voz activa, es un recado hablado; sin ninguna voz, es una notificación en pantalla.
- **Hablar de las tareas**: incluye lo vencido y lo que vence hoy en tus listas.
- **Hablar de las reuniones**: incluye las citas de hoy, si [la agenda](agenda-e-reunioes) está
  conectada.

Debajo de los interruptores, la sección **Hoy** muestra de qué hablaría si abrieras la app ahora,
proyecto por proyecto. Sin nada pendiente en ningún proyecto, no dice nada.

Cada uno de los dos interruptores de contenido avisa cuando el grupo de herramientas correspondiente
está apagado en Ajustes → Herramientas: Nina menciona la tarea o la reunión, pero no puede actuar
sobre ellas por voz.
