---
slug: o-modo-comando
titulo: El modo comando
resumo: Mantener ⌥X y decir una orden: qué acepta, qué rechaza y cómo la frase se vuelve acción.
area: nina
nivel: basico
---

**⌥X**: mantén la tecla, di la orden, suelta. La tecla se cambia en **Ajustes → Atajos**, en la fila
"Comandar".

El comando ejecuta y confirma en una frase corta. No abre conversación y no escucha tu respuesta. Para
conversar, usa [Nina por voz](falar-com-a-nina) (⌥C); para escribir un texto dentro de un agente, usa
[el dictado](ditado) (⌥D).

**El modo comando entiende portugués**, y solo portugués. La interfaz de la app habla español,
portugués e inglés, y [el dictado](ditado) sigue el idioma elegido, pero las órdenes habladas se
interpretan en portugués. Una orden dicha en otro idioma no se ejecuta, así que los ejemplos de abajo
son las frases que funcionan.

## Qué se puede ordenar

Las mismas herramientas de Nina, en la lista de
[lo que ella puede hacer](o-que-ela-consegue-fazer). Ejemplos que funcionan tal cual:

```
"abre um agente"                      "sobe dois agentes"
"ei Freya, roda os testes"            "pede pro Apolo revisar o login"
"chama a Freya de volta"              "quais agentes existem?"
"quem foi que mexeu no pagamento?"    "como estamos?"
"abre o git"                          "fecha o browser"
"coloca o browser em foco"            "me leva até a Gerda"
"anota aí que eu preciso arrumar o login"
"organiza as janelas uma embaixo da outra"
"troca o tema pra forja"              "põe um fundo de floresta"
```

### Varias órdenes en una frase

Una frase puede llevar tantas órdenes como digas, y se ejecutan en el orden en que aparecen:

```
"fecha o Apolo e organiza em duas colunas"
"bom dia! fecha a Gerda, abre dois agentes, põe em duas colunas e mostra o status"
```

Los saludos no cuentan como orden, y la misma orden dicha de dos maneras ("minimiza o vídeo, quero só
o áudio") sigue siendo una.

### Cuando no hay ninguna orden

Frases como "testando, você está me ouvindo?" reciben una respuesta corta y no pasa nada en pantalla.
No entender y que no haya orden son cosas distintas: en el segundo caso la app responde en una frase,
en lugar de inventarse una acción.

## Qué rechaza

Toda orden pasa por una comprobación antes de ejecutarse, y cuatro cosas son imposibles:

- **Cerrar sin un verbo de cerrar en tu frase** ("fecha", "tira", "apaga", "dispensa", "limpa").
- **Cerrar todo sin la palabra "tudo"**.
- **Crear un agente sin un verbo de creación.** Decir la palabra "agente" no basta: "põe os agentes em
  três colunas" no crea a nadie.
- **Mandar cualquier cosa a un agente cuyo nombre no pronunciaste.**

Cuando una de estas trabas bloquea algo, el motivo queda registrado en el diario de la voz, en Ajustes
→ Diagnóstico.

## Cómo la frase se vuelve acción

Tu habla se transcribe en tu propio Mac, y de aquí solo sale el texto. Quien interpreta el texto es el
modelo elegido en **Ajustes → Voz → Modelo del comando**, que depende de la clave de OpenAI. Sin
clave, sin red o sin respuesta a la petición, un modelo del propio Mac toma el relevo, y después de él
un enrutador de palabras clave.

El modo comando cuesta una fracción de un turno de conversación. Ver
[cuánto cuesta](quanto-custa).

## Qué ves y qué oyes

- Mientras la tecla está pulsada, una ventanita muestra el texto que se transcribe.
- Cuando la orden va a un agente, una chispa cruza el lienzo hasta su panel, mostrando a qué agente
  la mandó la app.
- La confirmación se habla con la voz natural, o con la del sistema cuando esa está apagada. La voz
  empieza cerca de un segundo después; la acción ya ocurrió antes.
- **Esc** cancela el comando en curso.
