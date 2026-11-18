# Instalar el juego en el móvil (PWA)

Archivos: `manifest.webmanifest`, `sw.js`, carpeta `icons/` (icono 64/192/512, maskable y apple-touch) y las metaetiquetas del `<head>` de `index.html`.

## Cómo publicarlo
El service worker (juego sin conexión) y la instalación **solo funcionan con HTTPS** (o `localhost`). Abrir `index.html` como archivo (`file://`) sigue funcionando para jugar, pero sin instalación.

Sube **toda la carpeta `Juego/`** (index.html, sw.js, manifest.webmanifest, icons/) a cualquier alojamiento estático con HTTPS: GitHub Pages, Netlify, el espacio web de la universidad, etc. Mantén los archivos en la misma carpeta (las rutas son relativas).

## Cómo instalarlo
- **Android (Chrome):** menú ⋮ → «Instalar aplicación» (o «Añadir a pantalla de inicio»).
- **iPhone/iPad (Safari):** botón Compartir → «Añadir a pantalla de inicio».
- **Escritorio (Chrome/Edge):** icono de instalar en la barra de direcciones.

## Notas
- Tras la primera visita con conexión, el juego se guarda en caché y funciona sin red. La tipografía pixel viene de Google Fonts: se cachea en esa primera visita; si no hay caché usa una tipografía monoespaciada.
- Para publicar una versión nueva, cambia `CACHE='siesta-v1'` en `sw.js` (por ejemplo a `siesta-v2`). `index.html` se pide primero a la red, así que las actualizaciones llegan solas cuando hay conexión.
- El progreso, los logros y el nombre del diploma se guardan en el navegador del dispositivo; usa «PARTIDAS» para exportarlos o pasarlos de un dispositivo a otro.
