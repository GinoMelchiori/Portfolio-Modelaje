# Portfolio de modelo

Sitio web personal para mostrar un portfolio de modelo: galería por categorías (colecciones, colaboraciones, sesiones de fotos y desfiles), sección «Sobre mí» editable, apartado de polaroids y contacto.

Hecho con **HTML, CSS y JavaScript puro** (sin frameworks ni dependencias). Responsive y con modo claro/oscuro automático.

## Estructura

```
index.html          Estructura de la página
styles.css          Estilos (responsive + tema claro/oscuro)
app.js              Lógica: edición, galería, polaroids, lightbox
data/portfolio.json Contenido publicado (se carga si el navegador no tiene datos propios)
```

## Uso

1. Abrí `index.html` en el navegador, o publicá el repo con **GitHub Pages** (Settings → Pages → rama `main`).
2. Agregá `#editar` al final de la URL (`.../index.html#editar`) para mostrar los botones de edición.
3. Cargá fotos, textos y datos. Todo se guarda en el `localStorage` del navegador y las imágenes se comprimen automáticamente.

## Publicar tu contenido para todos

El `localStorage` es privado de cada navegador, así que para que los visitantes vean tu contenido:

1. En modo edición, tocá **Exportar** (descarga `portfolio.json`).
2. Reemplazá `data/portfolio.json` del repo por ese archivo y hacé commit.
3. Los visitantes verán tu contenido al abrir la página. **Importar** carga un archivo exportado en otro navegador.

## Funcionalidades

- Edición en el lugar de nombre, frase, historia, medidas y contacto
- Galería con filtros por categoría y visor a pantalla completa
- Polaroids con epígrafes editables
- Compresión de imágenes en el navegador
