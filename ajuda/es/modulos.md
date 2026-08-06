---
slug: modulos
titulo: Crear un módulo
resumo: La carpeta, el manifiesto, las acciones que se vuelven herramientas de voz y qué puede hacer la página con el puente de la app.
area: modulos
nivel: avancado
---

Un módulo es una carpeta en `Application Support/codeCanvas/modulos/<id>/`, y el nombre de la carpeta
es el id del módulo. Dos piezas son obligatorias: `modulo.json` e `index.html`. Cómo se comporta una
vez listo está en [el panel de un módulo](painel-modulos).

No hay instalador ni registro: la app vigila la carpeta. Crearla hace aparecer el módulo, corregirla
lo trae de vuelta, borrarla lo saca de la app.

## Pedírselo a un agente

Pídeselo a un agente del lienzo: *"crea un módulo que muestre el saldo de mi cuenta del banco X"*. Él
estampa la carpeta con el esqueleto, la edita, abre el panel, le saca una foto, lee la consola y
corrige.

El esqueleto viene con el manifiesto rellenado, una página que ya usa el puente, un script de ejemplo
ya declarado como acción, y el archivo `CONTRATO.md` con la referencia completa en la versión de esta
app.

El id sale del nombre, en minúsculas, sin acentos ni espacios. Un nombre que choque con un panel
nativo de la app es rechazado, y un id que ya exista también.

## El manifiesto

- **`formato`**: la versión del contrato. Obligatorio, y hoy es `1`. Un formato mayor que el que la
  app conoce se rechaza entero, con el motivo.
- **`nome`**: obligatorio. Es el nombre en el panel, en el `⌘K` y en la voz.
- **`descricao`**: la línea debajo del nombre en el catálogo y en la barra del panel.
- **`icone`**: un símbolo de SF Symbols.
- **`palavras`**: sinónimos que acepta la búsqueda del `⌘K`.
- **`varios`**: `true` permite más de un panel de este módulo por lienzo.
- **`usaContexto`**: documenta que el contenido varía por proyecto. No cambia el comportamiento de la
  app.
- **`recarregarACada`**: recarga la página sola cada N segundos, mínimo 5.
- **`semMoldura`**: `true` hace que el panel suelto esconda cabecera y borde.
- **`acoes`**: las herramientas que el módulo le da a Nina y a los agentes.

## Las acciones

Cada acción tiene un **`nome`** (minúsculas, números y `_`), una **`descricao`** y un **`script`** de
su propia carpeta. Al ser llamada, la app ejecuta el script y devuelve la salida estándar a quien la
llamó; Nina responde hablando sobre ella.

La `descricao` es el campo que decide cuándo se llama la acción: escribe qué hace, qué devuelve y en
qué pedido usarla. Vaga, se la llama en el momento equivocado, o nunca.

La salida tiene que ser corta y legible. Los errores van a la salida de error, con código de salida
distinto de cero, y eso es lo que la app pasa como fallo.

Nina recibe las acciones en la apertura de la conversación: encender o apagar el interruptor de un
módulo vale a partir de la conversación siguiente. Los dos interruptores están en
[el panel de un módulo](painel-modulos).

## Qué puede hacer la página

La página recibe un puente hacia la app: petición sin restricción de origen, ejecutar un script de la
carpeta, saber en qué proyecto está, adoptar el tema, guardar datos y avisarte. Está en
[las capacidades de un módulo](modulos-capacidades).

## Por dónde seguir

- El concepto: [qué es un módulo](modulos-o-que-e).
- El panel en la pantalla y la lista en Ajustes: [el panel de un módulo](painel-modulos).
