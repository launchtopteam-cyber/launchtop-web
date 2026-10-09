# Launch Top™ — web

Código fuente de https://launchtop.es, ahora versionado en GitHub y conectado a Vercel.

## Qué hay en esta carpeta

| Archivo | Qué es |
|---|---|
| `index.html` | La web completa (autocontenida, con logos incrustados) |
| `robots.txt` | Permisos para Google + crawlers de IA (GPTBot, Gemini, Claude, Perplexity) |
| `sitemap.xml` | Mapa del sitio para buscadores |
| `llms.txt` | Ficha de la empresa para motores de IA generativa (GEO) |
| `og.png` | Imagen que sale al compartir el link en WhatsApp/LinkedIn/etc. (pendiente de resubir) |
| `vercel.json` | Configuración de Vercel (cabeceras de seguridad y caché) |

## Flujo de trabajo a partir de ahora

Este repo está conectado al proyecto `launchtop` en Vercel. Cualquier cambio que se suba
(push) a la rama `main` se despliega automáticamente a `https://launchtop.es`.

1. Edita los archivos en `src/`.
2. `git add -A && git commit -m "describe el cambio"`.
3. `git push`.
4. En ~30-60s el cambio está en producción.

## Dominio

Todo está configurado para `https://launchtop.es` (canonical, Open Graph, sitemap, robots y
llms.txt). No hay que tocar nada de eso salvo que cambie el dominio.

## Blog

La sección de blog vive en `src/blog/` (se añade en un commit posterior a este). Cada entrada
es un archivo HTML independiente enlazado desde `sitemap.xml`.
