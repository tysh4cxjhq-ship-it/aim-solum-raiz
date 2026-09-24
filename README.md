# aim-solum-raiz

La raiz `aim-solum.ai` redirige a `https://www.aim-solum.ai`, que es donde vive AIM SOLUM (Railway).

Por que existe: GoDaddy no admite CNAME en la raiz y su reenvio no se puede activar con nuestro token de API
(la API v2 responde ACCESS_DENIED). Railway sirve la raiz por https pero rechaza el http (solo pasa a https los
dominios cuyo CNAME ve). GitHub Pages da IPs fijas para registros A, certificado propio y paso de http a https.

- `index.html` y `404.html`: redirigen conservando ruta, parametros y ancla (y sin JavaScript, a la portada).
- `CNAME`: el dominio propio.

Mantenimiento: ninguno. Si algun dia el DNS pasa a un proveedor con CNAME en la raiz (p. ej. Cloudflare),
este repositorio sobra.
