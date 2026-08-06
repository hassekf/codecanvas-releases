---
slug: ajustes-navegador
titulo: Página de inicio del navegador
resumo: En qué dirección abre un navegador nuevo en este proyecto, y cuándo esa elección no vale.
area: projeto
nivel: basico
---

En **Editar "nombre del proyecto"… → Navegador**. La pestaña tiene un control: **Página de inicio**.

## El campo

- **Qué acepta**: la dirección tal como la escribe una persona. `github.com` se convierte en
  `https://github.com`, `localhost:3000` funciona, y una dirección que ya empiece por `http://` o
  `https://` pasa tal cual.
- **La línea de debajo del campo** muestra en qué dirección abrirá de verdad, y cambia mientras
  escribes, sin necesidad de guardar.
- **En blanco, abre Google.**

La elección es de cada proyecto, y nada se graba hasta que guardas la hoja.

## Cuándo vale

Vale para el navegador que **tú** abres, por el `⌘K` o por el catálogo de paneles, y para el que la
asistente de voz abre a petición tuya.

**No** vale para el navegador que un agente abre para enseñarte algo: ese ya viene con una dirección.
Ver [el panel del navegador](painel-navegador) y
[el agente ve el navegador](o-agente-ve-o-navegador).

## La otra elección sobre navegador

La pestaña **Agentes** del mismo proyecto tiene el **Navegador predeterminado**, con dos opciones:

- **Interno**: el agente muestra lo que produjo en el navegador de dentro del lienzo. Es el
  predeterminado.
- **Externo**: el agente abre en tu navegador del sistema, y solo usa el de dentro cuando se lo
  pides.

Aquella responde dónde muestra el agente; esta responde en qué página abre un navegador vacío. El
detalle está en [ajustes de agentes](ajustes-agentes).
