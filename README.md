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

## Publicar (Vercel)

El sitio se publica con Vercel CLI, directo desde esta carpeta:

```bash
vercel deploy --prod --yes
```

Queda disponible en: `https://indexpilot-demo.vercel.app/`

> Nota: originalmente se intentó GitHub Pages, pero un outage de GitHub Actions
> (2026-07-19) bloqueó los deploys y se migró a Vercel. El repo en GitHub sigue
> siendo el origen del código; Vercel solo hostea.

## Importante

Si cambiás el nombre del repo o el usuario, hay que actualizar las URLs en `sitemap.xml`,
`robots.txt` y las etiquetas `<link rel="canonical">` de cada página.
