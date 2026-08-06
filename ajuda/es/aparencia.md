---
slug: aparencia
titulo: La apariencia del proyecto
resumo: Tema, paisaje de fondo, velo, fondo de pantalla y fuente de la interfaz, elegidos por proyecto.
area: canvas
nivel: basico
---

Todo lo de esta página se elige en la pestaña **Apariencia** de la hoja de editar el proyecto: abre
el selector de proyecto en la barra de abajo y haz clic en **Editar "nombre del proyecto"…**. En la
pantalla de inicio, al mismo sitio se llega por el "⋯" de la tarjeta del proyecto o con clic derecho
sobre ella. El recorrido por los controles está en [apariencia del proyecto](ajustes-aparencia).

La elección es de cada proyecto. Cambiarla aquí no toca ningún otro.

## Los temas

Son diez, uno por tarjeta: Meia-noite (el predeterminado), Grafite, Forja, Bosque, Ameixa, Enseada,
Rubi, Aurora, Terracota y Marfim. Sus nombres están en portugués en todos los idiomas. La vista
previa de la tarjeta muestra el fondo de ese tema, un panel de vidrio encima y las tres señales de
estado de los agentes.

Hacer clic en la tarjeta aplica el tema en la pantalla al instante. Nada se graba hasta que guardas
la hoja, y cerrar sin guardar devuelve lo que había.

**Marfim** es el único claro: convierte toda la interfaz al lado claro. Dos consecuencias:

- **El rectángulo donde escribe el agente sigue oscuro.**
- **La pantalla de inicio sigue oscura**, por ser anterior a cualquier proyecto.

## El paisaje del tema

Cada tema trae su propio paisaje, que viene dentro de la app y no se descarga. Los tres botones de la
tarjeta eligen qué hacer con él:

- **Animado**: el vídeo del paisaje, en bucle y mudo. Es el predeterminado. Queda no disponible en el
  tema que no tenga vídeo.
- **Parado** (fija): el paisaje congelado. Cuando el tema ofrece más de una escena, las miniaturas
  aparecen dentro de su tarjeta para que elijas cuál.
- **Só cor** (solo color): ningún paisaje, solo el degradado del tema.

Hacer clic en uno de esos botones en la tarjeta de otro tema cambia el tema y el estilo de una vez.
El estilo elegido vale para todos los temas; la escena elegida vale solo para el tema en vigor.

El vídeo se pausa solo cuando la ventana queda escondida tras otra app o se minimiza.

## El velo

El control **Oscuridad del velo** decide cuánto se atenúa el fondo para que el texto de los paneles
sobreviva encima de él. Vale para el paisaje del tema y para tu fondo de pantalla, y va del 0% al
100%; al 0% el fondo se ve tal cual.

- **Desaparece de la pantalla** cuando no hay ningún fondo, es decir, en el estilo "Só cor" sin fondo
  de pantalla.
- El botón **Predeterminado** aparece junto al número cuando el valor está fuera del predeterminado
  del tema en vigor.
- Cambiar entre un tema oscuro y Marfim **mueve el velo con él**, y solo mientras siga en el
  predeterminado del lado del que sales. Después de que lo toques una vez, ningún cambio de tema lo
  mueve.

## El fondo de pantalla

En el bloque **Personalizar el fondo** pones un archivo tuyo en lugar del paisaje. Nace recogida,
salvo que este proyecto ya tenga un fondo de pantalla.

- **Elegir archivo…** acepta imagen, GIF y vídeo (MP4, MOV y M4V). El vídeo y el GIF se reproducen en
  bucle y mudos. El archivo se **copia dentro de la carpeta de la app**, así que borrar el original
  después no borra el fondo.
- **Cambiar** lo sustituye, **Quitar** devuelve el paisaje del tema.
- Mientras haya un archivo tuyo, gana al paisaje del tema, y los botones Animado, Parado y Só cor
  dejan de cambiar lo que ves. El resto del tema sigue valiendo.

### Pedir un fondo en vez de elegir un archivo

El bloque **O pide uno**, dentro de la misma tarjeta, solo aparece con la clave de OpenAI guardada en
[configurar la voz](configurar-a-voz). Describes el fondo y eliges entre dos botones:

- **Buscar**: busca en la web una imagen que ya existe y devuelve una cuadrícula de candidatas para
  que hagas clic. Es rápido, y es el camino para algo específico y real.
- **Crear**: pinta una imagen a partir de la descripción. Tarda unos 40 segundos, cuesta unos
  céntimos de dólar, y viene de una en una.

## La fuente de la interfaz

El menú **Fuente de la interfaz** muestra cada opción escrita en su propia fuente, con una muestra
debajo. Vale para toda la app mientras este proyecto esté abierto.

La fuente de los **terminales** es otra, es de toda la app, y está en **Ajustes → Terminal**, junto al
tamaño.

## El vidrio de los paneles

Dos controles en **Ajustes → Interfaz** deciden cuánto se ve el lienzo detrás del texto de los
paneles. Valen para toda la app, no para un proyecto.

- **Desenfoque del vidrio de los paneles**: cuánto desaparece el fondo detrás del panel. Avanza por
  escalones, porque así desenfoca el sistema.
- **Opacidad de los paneles**: la capa por encima del vidrio, del 0% al 100%. Subir la opacidad
  esconde el efecto del desenfoque.

## Por voz

Con la asistente configurada:

- *"cambia el tema a forja"*: los conoce los diez por nombre.
- *"pon un fondo de bosque con niebla"*: **pinta** por defecto. Decir "busca", "encuéntralo en
  internet" o pedir algo específico y real hace que busque en la web.
- *"busca otro"*: cambia por la siguiente candidata sin que repitas la descripción. Es instantáneo
  mientras haya candidatas guardadas.
- *"quita el fondo"*: retira el fondo de pantalla y devuelve el paisaje del tema.

Las tres primeras necesitan la clave de OpenAI.

Pedir una **imagen** es otra cosa: se pega en el lienzo y se guarda en la galería. Ver
[el panel de la galería](painel-galeria).
