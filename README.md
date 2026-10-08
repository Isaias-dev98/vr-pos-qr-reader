# Lector QR independiente del POS

Esta página estática se aloja en GitHub Pages para abrir la cámara fuera del marco de Google Apps Script. Sólo lee un QR y devuelve el texto a la pestaña del dashboard que la abrió mediante `postMessage`, con origen, ventana y sesión efímera validados.

No contiene catálogo, datos comerciales, credenciales ni muestras de códigos del negocio. El lector necesita abrirse desde el botón Cámara del Punto de venta; para cada apertura procesa una sola lectura y libera la cámara.

El decodificador jsQR se distribuye localmente en `jsqr.js`, sin CDN. La cámara requiere HTTPS y permiso del navegador.
