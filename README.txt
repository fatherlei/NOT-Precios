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
(no dentro de una subcarpeta). Borrá cualquier otro .html viejo que
haya quedado en el repo (por ejemplo copias tipo
"Calculadora_NOT_FINAL...") — el sitio solo usa index.html.

Esta versión usa Service Worker "not-app-v26" para invalidar la caché
anterior. Ese número de versión es lo que le avisa al teléfono/
navegador que hay contenido nuevo para descargar — si en el futuro
volvés a subir cambios y no se actualiza solo, subí también el número
de versión en la primera línea de service-worker.js.

DESPUÉS DE SUBIR LOS ARCHIVOS:
1. Esperá 1-2 minutos a que GitHub Pages termine el deploy.
2. Abrí la app y esperá unos segundos — el Service Worker nuevo se
   instala solo en segundo plano.
3. Cerrá completamente la app (o la pestaña) y volvé a abrirla. Recién
   ahí se activa la versión nueva y se borra la caché vieja.
   (Si seguís sin ver los cambios, borrá el acceso directo/ícono de
   la pantalla de inicio y agregalo de nuevo desde el navegador.)

SINCRONIZACIÓN CON GOOGLE SHEETS:
Esta versión de index.html sincroniza en una sola dirección: de la
app hacia tu Hoja de Google (nunca al revés, así tus datos locales
nunca se pisan). Andá a Ajustes, pegá la URL /exec de tu Web App de
Apps Script (Code.gs) y tocá "Guardar URL". Desde ahí, cada cambio
que guardes se sube solo; también hay un botón "🔄 Sincronizar ahora"
por si querés forzarlo.
