# Hoy toca vivir — paquete de distribución

## Opción A: abrir sin instalar
Abre `index.html` directamente. El juego no depende de archivos externos y conserva sus recursos embebidos.

## Opción B: experiencia tipo app en iPhone (recomendada)
Este paquete incluye `manifest.webmanifest`, `sw.js` e iconos para convertirlo en una PWA instalable.
Importante: Safari/iOS requiere que la PWA se sirva desde HTTPS (no funciona el service worker desde `file://`).
Una vez instalada y cacheada, el juego puede funcionar sin conexión.

Archivos:
- `index.html` — juego
- `manifest.webmanifest` — configuración de instalación
- `sw.js` — caché/offline
- `icon-180.png` y `icon-512.png` — iconos

El contenido original del juego se conserva; solo se añadió la capa de distribución para iPhone.
