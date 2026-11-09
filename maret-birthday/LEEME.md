# Happy Birthday, Maret — cómo subirla a Vercel

## Contenido de la carpeta
- `index.html` — toda la página
- `flowers/`, `img/`, `audio/` — fotos, imagen del pastel, notas de voz e instrumental
- `vercel.json` — configuración para Vercel (no hace falta tocarla)

## 1. Recibir el deseo de Maret (Formspree)
1. Crea una cuenta gratis en https://formspree.io
2. Pulsa **New Form**, ponle de nombre "Maret wishes" y elige tu correo.
3. Copia el link del formulario, algo como `https://formspree.io/f/abcdwxyz`
4. (Ya está puesto: https://formspree.io/f/myeeqzjd)
   `const WISH_ENDPOINT = "";`
   y pega tu link entre las comillas:
   `const WISH_ENDPOINT = "https://formspree.io/f/abcdwxyz";`
5. Guarda el archivo.

El deseo te llegará al correo y también lo verás en el panel de Formspree.

## 2. Subirla a Vercel

### Opción A — con GitHub (la más fácil de mantener)
1. Crea un repositorio nuevo en https://github.com/new (por ejemplo `maret-birthday`).
2. Pulsa **uploading an existing file** y arrastra TODO el contenido de esta carpeta
   (index.html, vercel.json, flowers, img, audio). Pulsa **Commit changes**.
3. Entra a https://vercel.com, inicia sesión con GitHub y pulsa **Add New… → Project**.
4. Elige el repositorio `maret-birthday` y pulsa **Import**.
5. En **Framework Preset** deja **Other**. No cambies nada más y pulsa **Deploy**.
6. Vercel te da un link como `maret-birthday.vercel.app`. Ese es el que le mandas a Maret.

Para actualizarla después: sube los archivos nuevos al mismo repositorio y Vercel se actualiza solo.

### Opción B — desde la terminal
1. Instala Node.js (https://nodejs.org).
2. Abre una terminal dentro de esta carpeta y escribe:
   `npx vercel`
   (te pedirá iniciar sesión; acepta las opciones por defecto)
3. Para publicarla en el link definitivo:
   `npx vercel --prod`

## 3. Probarla antes del 11 de noviembre
- La cuenta regresiva está activa hasta el 11/11 00:00 (hora de Chechenia) = 10/11 17:00 (hora de Bolivia).
- Para saltarla tú: toca **7 veces** la frase "not yet, Maret…".
- Apaga las velas y guarda un deseo de prueba para comprobar que te llega (luego bórralo en Formspree).
