---
slug: painel-git
titulo: El panel de Git
resumo: Las tres pestañas del repositorio: lo que está en tu carpeta, las issues y las pull requests, con lo que hace cada botón.
area: paineis
nivel: basico
---

El repositorio del proyecto en tres pestañas: **Git**, **Issues** y **PRs**. Cada pestaña muestra
cuántos elementos tiene; cuando la cuenta es cero, el número no aparece.

Ábrelo con `⌘K` escribiendo "git", o haciendo clic en el indicador de rama en el pie. El panel es
uno por lienzo: pedirlo de nuevo trae al frente el que ya existe.

## El indicador del pie

- **La rama actual**, truncada por el medio cuando es larga.
- **Flechas**: cuántos commits estás por delante y por detrás del remoto. Aparecen solo cuando hay
  divergencia.
- **La cuenta de archivos modificados**, con el total de líneas añadidas y quitadas, o la palabra
  "limpio" cuando no hay nada que confirmar.
- **"N disputados"**, cuando algún archivo modificado tiene más de un autor.
- **Hacer clic** abre este panel.

## La pestaña Git

La cabecera trae la rama, las flechas de divergencia con el remoto, el sello de la pull request de
esta rama y el botón de recargar. Sin un remoto configurado, las flechas no aparecen. Fuera de un
repositorio, la pestaña dice que el workspace no es un repositorio git.

- **Cambios**: los archivos modificados y aún no confirmados. Cada fila trae la letra del estado, la
  ruta, cuántas líneas entraron y salieron, y el nombre de quien tocó el archivo, incluso antes de
  cualquier commit. Tu propia edición en un [panel de archivo](painel-arquivo) cuenta como autoría.
- **Archivo disputado**: el que tiene dos o más autores recibe una alerta en su fila. El orden de la
  lista es conflictos primero, disputados después, y el resto por ruta.
- **Commits**: los 25 últimos, con resumen, autor y cuándo. El commit creado por un agente en esta
  sesión aparece con el nombre del agente; los demás muestran el autor registrado en git, que eres
  tú en todos ellos.
- **Diff**: hacer clic en un archivo modificado abre el diff en lugar de la lista. La flecha de la
  esquina superior vuelve atrás.

## La pestaña Issues

Las issues abiertas del repositorio.

Los botones de esta pestaña están rotulados en portugués, sea cual sea el idioma de la app.

- **El filtro de arriba** recorta por etiqueta. **Todas las issues** desactiva el recorte.
- **Hacer clic en una issue** despliega las acciones, las etiquetas y la descripción.
- **Trabalhar nisto** ("trabajar en esto"): abre un agente nuevo con la issue montada como primera
  tarea. Con más de un proveedor activado, el botón se convierte en un menú de cuál abrir.
- **Mandar para…** ("enviar a"): entrega la misma tarea a un agente ya abierto en este lienzo. Sin
  ningún agente abierto, el botón no aparece.
- **Fechar** ("cerrar"): marca la issue como resuelta en GitHub.
- **Abrir no app** abre la issue en un [panel de navegador](painel-navegador); **Abrir no GitHub**
  la abre en el navegador del sistema.

El texto entregado por **Trabalhar nisto** y por **Mandar para…** es el mismo, e instruye al agente
a comentar y cerrar la propia issue al terminar.

## La pestaña PRs

Las pull requests abiertas.

- **Todas** y **Esperándote**: la segunda recorta las que están detenidas en tu revisión.
- **Plegada**, cada fila trae número, título, el sello de la revisión (**Aprobada**, **Cambios**,
  **Pendiente**) y el de la CI, cuando la PR tiene CI.
- **Hacer clic** la despliega, y solo entonces la app busca la descripción y los archivos, que el
  listado no trae.
- **Aprobar**: pide confirmación y publica la aprobación en GitHub. Queda no disponible en una PR
  que ya aprobaste.
- **Comentar**: abre un campo de texto. **Enviar** publica un comentario suelto, que no se convierte
  en revisión.
- **Los archivos modificados** aparecen con el saldo de líneas de cada uno. Hacer clic en cualquiera
  de ellos abre los archivos de la PR en el navegador.

Fusionar y pedir cambios no existen en este panel.

## El sello de pull request

Cuando la rama de un agente ya se convirtió en PR, su número y el estado de la CI aparecen en el
panel del agente, en el pie y en la cabecera de la pestaña Git. Sin PR abierta, el sello no ocupa
espacio.

El interruptor es **Sello de pull request**, en
[configuración de los agentes](ajustes-agentes). Desactivado, no aparece ningún sello y la app deja
de consultar a GitHub sobre tus PRs.

## Qué exigen las pestañas Issues y PRs

Hablan con GitHub a través de `gh`, su herramienta de línea de comandos, usando la sesión que ya
existe en ella. Cuando algo falta, la pestaña dice cuál de las tres cosas es: `gh` no instalado,
`gh` sin sesión iniciada, o el proyecto sin un remoto de GitHub.
