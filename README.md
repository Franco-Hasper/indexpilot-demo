# IndexPilot — sitio de marketing

Sitio estático (HTML + CSS, sin dependencias) publicado con GitHub Pages.
Se usa como sitio real para probar el envío de URLs a la API de Indexación de Google.

## Estructura

```
index.html            Inicio
caracteristicas.html  Qué incluye el producto
precios.html          Planes
faq.html              Preguntas frecuentes
contacto.html         Contacto
sitemap.xml           Las 5 URLs de arriba
robots.txt            Permite rastreo + apunta al sitemap
styles.css            Estilos compartidos
```

## Publicar en GitHub Pages

1. Crear un repo **público** llamado `indexpilot-demo`.
2. Subir estos archivos a la rama `main`.
3. En el repo: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)`** → Save.
4. A los pocos minutos queda disponible en:
   `https://franco-hasper.github.io/indexpilot-demo/`

## Importante

Si cambiás el nombre del repo o el usuario, hay que actualizar las URLs en `sitemap.xml`,
`robots.txt` y las etiquetas `<link rel="canonical">` de cada página.
