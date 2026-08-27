# osessionsmusic.com

Press kit web de **O-Sessions** (Mario y Cristián Ojeda). Sitio estático de una
sola página, trilingüe (es/en/pt), sin dependencias externas: no carga
tipografías, ni librerías, ni analítica de terceros.

**Este repositorio es salida, no fuente.** No se edita a mano.

## De dónde viene

Se genera desde el repositorio de marca `O-Sessions`:

    node epk/build-epk.mjs --web

Los textos viven en `epk/data.json` y `epk/i18n.json`. El material de video se
recodifica con `PERFIL=web bash epk/encode-media.sh`.

## Cómo se publica una versión nueva

Desde el repositorio de marca:

    npm run deploy

Sincroniza `epk/web/` a este repositorio y empuja. GitHub Pages publica solo.

## Hosting

GitHub Pages sobre la rama `main`, dominio `osessionsmusic.com` con HTTPS
automático.
