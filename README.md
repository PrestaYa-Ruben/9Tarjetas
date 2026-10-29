# PrestaYa – Elige tu Carta (v3.0)

Juego PWA de 9 cartas con 2 oportunidades para ganar boletas adicionales para la rifa.

## Archivos
| Archivo | Para qué sirve |
|---|---|
| `index.html` | La app completa (juego, generador de enlaces, admin) |
| `manifest.json` | Datos de instalación: nombre, colores e íconos |
| `sw.js` | Service worker: carga rápida y uso sin internet |
| `icons/` | Íconos de la app (192, 512, maskable, iPhone y favicon) |
| `.nojekyll` | Evita que GitHub Pages procese los archivos |

## Publicar en GitHub Pages
1. Sube todos los archivos y la carpeta `icons` a la raíz del repositorio.
2. En el repositorio: **Settings → Pages → Branch: main / (root) → Save**.
3. Abre la dirección que te da GitHub Pages (https://usuario.github.io/repositorio/).

## Administrador
- 5 toques sobre el logo **PRESTAYA** + PIN para entrar al Generador.
- El PIN se cambia en `index.html`: `const ADMIN_PIN = "...";`
- El botón verde **⬇ App** (arriba a la izquierda) para instalar la app solo lo ve el administrador.
- Al actualizar la app, sube también `sw.js` con su versión nueva.
