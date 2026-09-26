# Portafolio — Nicolás Cubilla

Desarrollador de Software. Licenciado en Análisis de Sistemas Informáticos.

**Sitio publicado en:** https://nicolascubilla.github.io/Portafolioweb/

## Contenido

| Archivo | Descripción |
| --- | --- |
| `index.html` | Portafolio: perfil, experiencia, stack, proyectos y contacto |
| `cv.html` | Currículum en HTML, con foto y estilos de impresión |
| `CV-Nicolas-Cubilla.pdf` | Currículum en PDF (generado desde `cv.html`) |
| `img/` | Fotografía, capturas de los proyectos e imagen social |

## Cómo está hecho

Sitio estático, sin build ni dependencias. HTML y Tailwind CSS vía CDN, más un
script propio para el navbar, el resaltado de sección activa, las animaciones de
entrada y el efecto de escritura.

Todo el CSS y el JavaScript están en línea dentro de `index.html`, así que no hay
pasos de compilación: se edita y se recarga.

## Regenerar el PDF del CV

El PDF se genera desde `cv.html` con Chrome headless, de modo que siempre queda
sincronizado con el HTML:

```powershell
chrome --headless=new --disable-gpu --no-pdf-header-footer `
  --print-to-pdf=CV-Nicolas-Cubilla.pdf cv.html
```

Está pensado para ocupar una sola hoja A4. Si agregás contenido, verificá que no
se desborde a una segunda página.

## Contacto

- [LinkedIn](https://www.linkedin.com/in/nicolas-cubilla-137765269)
- [GitHub](https://github.com/nicolascubilla)
- [nicolascubillasosa2001@gmail.com](mailto:nicolascubillasosa2001@gmail.com)
