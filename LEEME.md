# Soul Digital Design · tienda de plantillas

Sitio estático de una sola página. No necesita servidor, base de datos ni instalación: se abre con doble clic y se publica arrastrando la carpeta a Netlify Drop.

## Qué hay en la carpeta

- `index.html` — la tienda: portada, catálogo, pedido, pagos y preguntas.
- `img/` — capturas de las plantillas (800 × 600, JPEG).
- `demo/` — las plantillas que se abren en la demo:
  - `cumpleanos.html`
  - `libro-familia.html`
- `cartas/` — la colección de cartas (6 estilos) con su propia página, sus demos y su formulario.
- `demo/extras/` e `img/extras/` — plantillas y capturas que no están en el catálogo, listas por si quieres cambiar la cuarta.

## Cambiar lo básico

Abre `index.html` y busca el bloque `CONFIG` (casi al final, dentro de `<script>`):

```js
const CONFIG = {
  marca: "Soul Digital Design",
  whatsapp: "5351321718",   // sin +, sin espacios, sin guiones
  moneda: "CUP",
  entrega: "24–48 h",
  ...
};
```

- **WhatsApp**: cámbialo por tu número. Todos los botones y el formulario lo usan.
- **Marca**: el nombre que aparece en la barra de arriba y en el pie.
- **Precios**: cada plantilla tiene `precio: 1000`. Es precio único en pesos cubanos (CUP).
- **Textos**: `nombre`, `desc` e `incluye` de cada plantilla.

## La cuarta plantilla

Ahora mismo el catálogo tiene tres plantillas reales y una tarjeta de “Tu propia idea”. Cuando me pases la cuarta, se cambia así:

1. Copia el archivo HTML a `demo/` (por ejemplo `demo/mi-plantilla.html`).
2. Toma una captura de 800 × 600 y guárdala en `img/` (por ejemplo `img/mi-plantilla.jpg`).
3. En `CONFIG.plantillas`, reemplaza el bloque de `\"Tu propia idea\"` por uno con su ruta y textos.

## Publicar en Netlify Drop

1. Entra a https://app.netlify.com/drop
2. Arrastra la carpeta completa `tienda-plantillas`.
3. Netlify te da un enlace tipo `https://algo.netlify.app`.

## Notas

- **Anticipación**: Se pide hacer los encargos con al menos **una semana de anticipación**.
- **Pago**: Únicamente por **transferencia** (CUP). Se reserva con el 50 % y el resto se paga al aprobar el borrador.
- **Negocio en crecimiento**: La cantidad y variedad de plantillas irá cambiando con el tiempo.
