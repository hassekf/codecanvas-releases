---
slug: busca-e-comandos
titulo: La búsqueda del lienzo
resumo: ⌘K: ir a un panel abierto, crear el que aún no existe, recuperar un agente y abrir una dirección.
area: canvas
nivel: basico
---

Se abre con **⌘K**, y la tecla vale incluso con el cursor dentro de un agente. Se cambia en
**Ajustes → Atajos**, en "Paleta de comandos".

## Las secciones del resultado

Los resultados vienen agrupados, y el grupo dice qué hará el Enter. Los títulos de las secciones
están en portugués en todos los idiomas.

- **Ir para** (ir a): lleva la cámara hasta un panel que ya está abierto. Ve los paneles de todas las
  áreas de trabajo, y elegir uno de otra área cambia de área también. Un panel minimizado no aparece.
- **Abrir** (abrir): crea un panel nuevo, a partir del catálogo. Solo aparecen los agentes de los
  CLIs activados en **Ajustes → Proveedores**.
- **Chamar de volta** (recuperar): recrea un agente que descartaste en este proyecto, con su
  conversación.
- **Ação** (acción): lo que tu frase pide sin nombrarlo. Organizar los paneles, crear un área de
  trabajo, volver a una disposición guardada, abrir una dirección.

Con el campo vacío, la lista trae solo la sección **Abrir**, ordenada por lo que más abres desde
aquí.

## Qué más encuentra

- **Las áreas de trabajo**, por nombre. Elegir una cambia de área.
- **Tus notas** de este proyecto, por título. Solo aparecen cuando las buscas.
- **Las disposiciones guardadas**, por el nombre que les diste. Ver
  [organizar el lienzo](organizar-sozinho).
- **Las ejecuciones en curso** de una iniciativa, por el nombre de la ejecución. Las terminadas no
  aparecen.

## La dirección escrita

Una URL completa abre tal cual. `github.com` se convierte en `https://github.com`. `localhost:3000` y
`127.0.0.1` abren por `http://`. Un número suelto entre 1024 y 65535 abre
`http://localhost:<número>`.

Un nombre de archivo no se convierte en dirección: `package.json` no abre en el navegador.

## Cómo se elige el resultado

- **Todo término escrito tiene que coincidir.** "browser medios" no devuelve los dos paneles,
  devuelve nada.
- **El verbo decide entre crear e ir.** "nuevo navegador" crea uno; "ve al navegador" lleva al que ya
  existe. Sin verbo, un panel abierto va antes que un panel por crear.
- **La grafía errónea se acepta** a partir de cuatro letras, y siempre por debajo de cualquier
  coincidencia exacta. "brwoser" encuentra el navegador.
- **Lo que más usas solo desempata**, entre dos resultados con la misma puntuación.
- **La etiqueta junto al nombre muestra el término que coincidió**, cuando no fue el título.

## Teclado

- **↑ ↓**: recorren la lista sin sacar el cursor del campo, y dan la vuelta al final.
- **Enter**: abre el resultado seleccionado.
- **Esc**: cierra.

## El recordatorio en lo alto del lienzo

La píldora en lo alto del lienzo muestra la tecla y no recibe clics. Se apaga en
**Ajustes → Interfaz**, en "Recordatorio del atajo de búsqueda"; apagada, lo alto queda solo con las
pestañas de las áreas. Su texto sigue al atajo que esté configurado.

## La búsqueda dentro de Ajustes

El campo **Buscar un ajuste**, en lo alto de la barra lateral de Ajustes, usa el mismo motor. Busca
en el título de cada ajuste, en la explicación de debajo y en las teclas de la app, y acepta términos
que no están escritos en la pantalla ("dark mode" lleva a Interfaz, "mic" al micrófono).

El resultado elegido no filtra la pantalla: abre la sección, desplaza hasta el ajuste y lo resalta
unos segundos. **↑ ↓** recorren la lista, **Enter** salta. **Esc** limpia el campo, y solo cierra
Ajustes cuando el campo ya está vacío.

## Qué no encuentra

No busca dentro de tus archivos ni dentro de lo que escribieron los agentes. Para eso, pídeselo a un
agente.
