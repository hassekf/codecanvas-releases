---
slug: modulos-o-que-e
titulo: Qué es un módulo
resumo: Un panel escrito por ti, que vive en el lienzo como los nativos y habla con la app.
area: modulos
nivel: avancado
---

Un módulo es **un panel tuyo**. Tú (o un agente tuyo) escribes una página, y pasa a vivir en el lienzo
como cualquier panel nativo: se abre con `⌘K`, entra en la disposición, se minimiza al estante y se
puede abrir por voz.

Sirve para lo que solo tiene sentido para ti: el saldo de una cuenta, el panel de una máquina que
administras, un contador a tu manera, la pantalla de un sistema interno que nadie más usa.

## Dónde vive

En una carpeta dentro de la carpeta de la app, una por módulo. Dos piezas son obligatorias: el
manifiesto, que declara qué es el módulo, y la página inicial.

**No hay instalador ni registro.** La app vigila la carpeta: crearla hace aparecer el módulo,
corregirla lo trae de vuelta, borrarla lo saca de la app. Mientras escribes, guardar un archivo
recarga los paneles de ese módulo sin reiniciar nada.

**El módulo es de tu máquina, no del proyecto.** Está disponible en todos los lienzos, y cada apertura
crea un panel de ese lienzo: la página sabe en qué proyecto está, y el mismo módulo puede mostrar
cosas distintas en cada uno.

## Qué gana por estar dentro del lienzo

Una página común en un navegador no consigue nada de esto:

- **Hacer una petición sin restricción de origen**, porque quien busca es la app.
- **Ejecutar un script de su propia carpeta**, con la salida de vuelta a la página.
- **Saber en qué proyecto está**, y adoptar el tema y la fuente de ese lienzo.
- **Guardar datos** entre aperturas y entre lienzos.
- **Avisarte** dentro de la app, con sonido, lectura en voz alta y un botón que te lleva al panel.
- **Darle herramientas a Nina y a los agentes**, para que usen el módulo hablando.

El detalle de cada una está en [las capacidades de un módulo](modulos-capacidades).

## Qué no es

- **No es una extensión de la app.** Dibuja dentro de su panel y no altera el resto de la interfaz.
- **No es distribuible.** No hay tienda, registro ni instalación por enlace: la carpeta es tuya.
- **No funciona sin ti.** Un módulo que necesita un secreto guarda el secreto en un script de la
  carpeta, y no en el HTML.

## Por dónde seguir

- Crear uno: [crear un módulo](modulos).
- El panel en la pantalla y la lista de módulos: [el panel de un módulo](painel-modulos).
