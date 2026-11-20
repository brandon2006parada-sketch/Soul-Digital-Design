# Cómo usar tu paquete de ventas

Carpeta: `C:\Users\pasto\Downloads\cartas-negocio`

| Archivo | Para qué sirve |
|---|---|
| `index.html` | Tu catálogo: demo en vivo, precios, preguntas y botones de WhatsApp. Es lo que compartes como "mi página". |
| `demo-amor.html` | Carta de muestra (San Valentín / amor). |
| `demo-cumple.html` | Carta de muestra (cumpleaños). |
| `demo-mama.html` | Carta de muestra (mamá / familia). |
| `plantilla-final.html` | Carta **limpia**, sin sellos de muestra ni botones de venta. De aquí sale cada pedido. |
| `guion-ventas.md` | Mensajes de WhatsApp, respuestas a objeciones, precios y publicaciones. |
| `guion-video.md` | Storyboard del video de 30 s y de 10 s. |

---

## 1. Tu WhatsApp (ya está configurado)

Tu número quedó puesto en los 4 archivos como `5351321718` (+53 51321718, Cuba).
Todos los botones abren `https://wa.me/5351321718` con el mensaje ya escrito.

Si algún día cambias de número, reemplaza `5351321718` en estos **4 archivos**:

- `index.html` (arriba del todo, en `const NEGOCIO = { whatsapp: ... }`)
- `demo-amor.html`
- `demo-cumple.html`
- `demo-mama.html`

En cada uno: abre con el Bloc de notas → Ctrl+H (reemplazar) → busca `5351321718` → reemplaza por el nuevo (sin +, sin espacios) → guardar.

En `index.html` también puedes poner tu Instagram y TikTok en la misma línea:

```js
instagram: "tuusuario",
tiktok: "tuusuario",
```

Si lo dejas vacío, esos enlaces se ocultan solos.

**Prueba antes de publicar:** abre `index.html`, toca "Quiero la mía" y verifica que abra tu chat de WhatsApp con el mensaje escrito.

---

## 2. Publícalo para tener un link (gratis, 3 minutos)

Un link vende mucho más que un archivo adjunto.

1. Entra a **https://app.netlify.com/drop** (no necesitas cuenta para probar).
2. Arrastra **la carpeta completa** `cartas-negocio`.
3. Te da una dirección tipo `https://algo-random.netlify.app`.
4. Prueba en tu celular: catálogo + las tres demos + botón de WhatsApp.
5. Si quieres un nombre bonito, crea una cuenta gratis y cambia el nombre del sitio (ej. `cartas-para-ti.netlify.app`).

> El link del catálogo es tu **prueba pública**. Compártelo en tu bio de Instagram/TikTok y en el estado de WhatsApp.
> Las demos también se pueden abrir como archivo, pero el link se siente producto.

---

## 3. Tu rutina de venta (todos los días, 15 minutos)

1. Publica un video o una historia con la carta (usa `guion-video.md`).
2. Cuando alguien pregunte, manda el link del catálogo, no el archivo.
3. Haz las 4 preguntas del guion (para quién, ocasión, fecha, recuerdos).
4. Cotiza con **dos** opciones, no con una.
5. Cierra con fecha: "te mando el borrador hoy, la tienes mañana".

---

## 4. Cómo producir una carta (20 minutos)

1. Copia `plantilla-final.html` y renómbralo, por ejemplo `carta-para-ana.html`.
2. Ábrelo con el Bloc de notas.
3. Busca `const CARTA = {` (línea ~74) y edita solo los textos entre comillas:
   - `saludo`: "Para Ana,"
   - `parrafos`: cada línea entre comillas es un párrafo
   - `firma`: "Tuyo, siempre. — Luis"
   - `deseo`: lo que aparece cuando sopla la vela
   - `aviso`: déjalo en `""` (vacío)
4. Guarda y ábrelo en el navegador para revisar.
5. Súbelo y manda el link.

**Ojo:** no borres las comillas ni las comas. Si algo se rompe, vuelve a copiar la plantilla.

---

## 5. Qué entregar y qué NO entregar

**Entrega:**
- El link (puedes subir cada carta a Netlify con otro nombre, o crear subcarpetas).
- Un **video de 15 s** grabado con el celular mostrando la carta ya personalizada. Es el respaldo emocional y además sirve como testimonio.
- Opcional: captura en PDF o imágenes por si el link falla.

**No entregues:**
- El archivo HTML editable antes de cobrar.
- La plantilla base ni las demos con el sello "MUESTRA".
- Tu carpeta completa de trabajo.

**Antes de entregar, revisa que la carta final NO tenga:**
- El sello `MUESTRA` (es el `<div class="marca">MUESTRA</div>`)
- El botón "Quiero una así" (`id="pedir"`) ni el de la pantalla del deseo (`id="pedir2"`)
- El bloque `const VENDEDOR = { ... }` del final

La `plantilla-final.html` ya viene limpia: úsala siempre como base y no tendrás que borrar nada.

---

## 6. Precios

Están en `index.html`, en la sección de precios (`US$9`, `US$19`, `US$35`).
Ajusta al mercado de tu país. La referencia funciona así:

- **Esencial** barato: atrae a los que dudan.
- **Personalizada** al medio: el 70 % elige este. Es el que te conviene vender.
- **Premium** alto: hace que el del medio parezca razonable.

También puedes cambiar el texto de cada plan y la nota de pago.

---

## 7. Protege tu trabajo

- El sello **MUESTRA** y los nombres ficticios hacen que la demo no sirva como producto final.
- Entrega el link, no el archivo, hasta que esté pagado.
- Si un cliente desaparece, no publiques su carta personalizada.
- Guarda una copia de cada carta entregada (te sirve como portafolio, con permiso).

---

## 8. Checklist antes de compartir el link

- [ ] Mi número de WhatsApp está en los 4 archivos
- [ ] Probé el botón desde el celular y abre mi chat
- [ ] Las 3 demos cargan y se escucha el sonido de la pluma
- [ ] La vela se apaga al tocarla y aparece el deseo
- [ ] El catálogo se ve bien en el celular (no solo en la compu)
- [ ] Ya publiqué el video de 30 s
- [ ] Tengo claro qué digo cuando me preguntan el precio

---

## 9. Errores que te van a costar ventas

1. **Mandar el archivo en vez del link.** Se ve como borrador y se puede reenviar gratis.
2. **Explicar la técnica.** A nadie le importa el HTML; le importa lo que siente la persona.
3. **No mostrar el sonido.** El video sin sonido pierde la mitad del efecto.
4. **Cobrar sin anticipo.** Con montos bajos, cobra el 100 % o al menos el 50 %.
5. **Aceptar "te aviso".** Siempre pon fecha y cupo: "te reservo hasta las 8 pm".
6. **No pedir testimonio.** La primera reacción real vale más que 10 publicaciones tuyas.
