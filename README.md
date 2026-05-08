# formula100k-ig-assets

Repositorio público que aloja imágenes y videos para que Zapier MCP pueda publicarlos en Instagram for Business desde Claude Code (skill `/publicar-ig`).

## Estructura

```
posts/
  YYYY-MM-DD-<slug>/
    image.png            # foto única
    video.mp4            # reel
    slide-01.png ...     # carrusel ordenado
```

Cada carpeta = una publicación. Las URLs raw.githubusercontent.com de estos archivos son las que Instagram recibe vía Zapier.

## Por qué público

Instagram (vía Graph API que usa Zapier) requiere URLs HTTPS accesibles públicamente para descargar la media. GitHub raw es la opción más simple, gratis y permanente.

## No tocar manualmente

Este repo lo administra la skill `/publicar-ig` en `~/.claude/skills/publicar-ig/SKILL.md`. Borrar carpetas viejas está bien (Instagram ya tiene su copia interna), pero no muevas archivos a mitad de una publicación.
