NOT — paquete completo para GitHub Pages / PWA

SUBIR TODO (reemplazando lo que ya está en el repo):
- index.html
- manifest.json
- service-worker.js
- logo.png
- icon-192.png
- icon-512.png
- README.txt

IMPORTANTE:
Todos los archivos deben quedar en la RAÍZ del repositorio de GitHub
(no dentro de una subcarpeta).

Esta versión usa Service Worker "not-app-v20" para invalidar la caché
anterior ("not-app-v19"). Es el número de versión el que le avisa al
teléfono/navegador que hay una versión nueva para descargar — si en el
futuro volvés a subir cambios y no se actualiza solo, subí también el
número de versión en la primera línea de service-worker.js.

DESPUÉS DE SUBIR LOS ARCHIVOS:
1. Esperá 1-2 minutos a que GitHub Pages termine el deploy.
2. Abrí la app y esperá unos segundos — el Service Worker nuevo se
   instala solo en segundo plano.
3. Cerrá completamente la app (o la pestaña) y volvé a abrirla. Recién
   ahí se activa la versión nueva y se borra la caché vieja.
   (Si seguís sin ver los cambios, probá desinstalar y volver a
   agregar el acceso directo/ícono a la pantalla de inicio.)

CAMBIOS DE ESTA VERSIÓN:
- Service Worker actualizado a v20 para forzar la actualización de
  caché en todos los dispositivos.
