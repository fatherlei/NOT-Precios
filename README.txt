NOT — paquete completo para GitHub Pages / PWA

SUBIR TODO:
- index.html
- manifest.json
- service-worker.js
- logo.png
- icon-192.png
- icon-512.png
- README.txt

IMPORTANTE:
Todos los archivos deben quedar en la RAÍZ del repositorio de GitHub.

Esta versión usa Service Worker "not-pwa-v3" para invalidar la caché anterior.
Después de subir los archivos, esperá a que GitHub Pages termine el deploy y
recargá la aplicación.

CAMBIOS DE ESTA VERSIÓN:
- Inicio: últimos pedidos registrados primero.
- Pedidos: próximos vencimientos primero.
- Entregados: tarjeta gris/atenuada y al final.
- PWA: manifest y Service Worker incluidos.
- Caché versionada para que las actualizaciones lleguen al teléfono.
- Logo e iconos incluidos localmente.
