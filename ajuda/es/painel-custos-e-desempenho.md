---
slug: painel-custos-e-desempenho
titulo: Uso y rendimiento
resumo: Dos paneles: cuánto de la suscripción de cada proveedor se ha ido y cuánto costó cada agente, y cuánta memoria y CPU usa la app, por proceso.
area: paineis
nivel: basico
---

El panel de uso se abre con `⌘K` (escribe "uso", "consumo" o "limite"); el de rendimiento, con
"desempenho", "cpu" o "memória".

## El panel de uso

Un bloque por proveedor con límite conocido. En cada bloque:

- **Las ventanas de límite** de la suscripción, cada una con el porcentaje ya gastado y cuándo se
  reinicia. El anillo mayor repite la ventana más ajustada, que es la que detiene el trabajo
  primero.
- **El plan**, cuando el proveedor lo informa.
- **Los créditos**, cuando existen: cuánto se usó y el tope, en la moneda de la cuenta. Siguen
  valiendo después de que una ventana se agota.
- **visto**: cuándo se leyó ese número por última vez. Los proveedores que solo publican el consumo
  al ejecutar una sesión pueden estar mostrando un número de hace días.

Debajo de los bloques, una línea atenuada con un **guion** lista los proveedores cuyo consumo no se
puede leer: Gemini, Cursor y Grok. El guion quiere decir "no lo sé", y no cero.

### En este lienzo

En **EN ESTE CANVAS**: el total gastado por los agentes de este lienzo, y una fila por agente con el
nombre que le diste. La barra de cada uno es proporcional al mayor gasto del lienzo, no a un valor
absoluto.

El valor es **estimado**: el precio no viene de la conversación, viene de una tabla de precios
incorporada.

### Cuentas separadas cuentan por separado

Un límite es de la cuenta, no del proyecto. Con más de una cuenta del mismo proveedor en uso, cada
una tiene su propio bloque, rotulado con el nombre de la cuenta. Lo que consume un lienzo cuenta
contra la misma cuenta en todos los demás. Ver [cuentas y perfiles](contas-e-perfis).

### Las cápsulas del pie

Una cápsula por proveedor en uso, con dos mitades en las que se puede hacer clic:

- **El logo del proveedor**: cambia de aspecto según el servicio esté en pie o con una incidencia.
  Hacer clic abre la página de estado de ese proveedor en un panel de navegador aquí dentro.
- **El anillo con el porcentaje**: la ventana más ajustada de esa cuenta. Hacer clic abre el panel
  de uso.

Con más de una cuenta a la vista, la inicial del nombre de la cuenta aparece antes del anillo.

Lo que gastan la asistente y la voz es otra cuenta, y está en [cuánto cuesta](quanto-custa).

## El panel de rendimiento

Mide la app, los agentes, los servidores que los agentes levantan y los navegadores, incluso con el
panel cerrado.

- **MEMÓRIA** y **CPU DA MÁQUINA**: los dos números actuales, con el gráfico de los minutos
  anteriores.
- **La línea bajo los números** compara con lo normal: o bien **no normal deste app**, o cuántas
  veces lo normal está pesando la app ahora. Es la desviación, y no el número, lo que dispara un
  informe.
- **DÓNDE ESTÁ LA MEMORIA**: el reparto por papel, entre **O app**, **Agentes**, **Servidores dos
  agentes**, **Browsers** y **Terminais**.
- **QUIÉN ESTÁ TIRANDO**: los seis procesos más pesados, con el nombre del panel al que pertenece
  cada uno.
- **Guardar informe**: escribe ahora un informe con todo lo que está pasando y lo abre en un panel.

Cuando el sistema no deja identificar qué procesos de WebKit son de la app, el panel avisa de que
los navegadores **no** entran en la cuenta.

### El número en la barra

Junto al zoom está la memoria en uso, y el porcentaje de CPU cuando pasa del 10%. Toma color al
acercarse a tu umbral de pico. Hacer clic abre el panel de rendimiento. Desaparece con el monitor
apagado.

### Qué cuenta como pico

En **Configuración → Rendimiento**.

- **Medir y guardar informes de pico**: activa el monitor. Apagado, no se mide nada, no se guarda
  ningún informe, el panel muestra un botón para volver a activarlo y el número sale de la barra.
- **Sensibilidade**: de +10% a +200% por encima de lo que la app suele pesar. La pantalla traduce el
  porcentaje al número de hoy ("aviso acima de X"), y lo normal se aprende en cerca de un minuto con
  la app abierta.
- **Abrir la carpeta** y **Ver el último**: la carpeta de los informes, y el informe más reciente en
  un panel.

Cada pico se convierte en un archivo con los procesos, los agentes, lo que estaba abierto y los
minutos anteriores. Se guardan los 30 más recientes, y ninguno sale de tu máquina.
