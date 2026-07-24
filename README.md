# Tienda Online - Proyecto Bootstrap

**Diseñado por:** [Tu Nombre Completo]
**Carné:** [XXXXXXXXX]

## Descripción del proyecto

Página web que simula una tienda en línea, construida con **HTML5** y **Bootstrap 5.3**. El proyecto incluye un encabezado con carrusel de imágenes, un ícono de carrito de compras (visual, no funcional), un menú de categorías, una sección de productos con tarjetas (cards) y un diseño totalmente responsivo.

## Componentes de Bootstrap utilizados

- **Navbar** (`navbar`, `navbar-dark`, `sticky-top`) para el encabezado principal.
- **Carousel** (`carousel`, `carousel-inner`, `carousel-item`, `carousel-indicators`) para el banner de imágenes en la parte superior.
- **Grid system** (`container`, `row`, `col-sm-3`, `col-sm-9`, `row-cols-1`, `row-cols-md-3`) para la distribución responsiva del cuerpo.
- **Cards** (`card`, `card-img-top`, `card-body`, `card-title`) para mostrar cada producto.
- **List group** (`list-group`, `list-group-item`) para el menú de categorías.
- **Buttons** (`btn`, `btn-warning`, `btn-outline-light`) para las acciones de "Agregar al carrito" y el botón del carrito.
- **Badge** (`badge`, `rounded-pill`) para el contador visual del carrito de compras.
- **Bootstrap Icons** para los íconos del carrito, tienda y categorías.

## Estructura de archivos

```
tienda-online/
├── index.html
├── css/
│   └── estilos.css
└── README.md
```

## Diseño responsivo

- En pantallas pequeñas (celulares): los productos se muestran uno por fila (`row-cols-1`).
- En pantallas medianas o grandes: los productos se muestran tres por fila (`row-cols-md-3`).
- El menú de categorías y la sección de productos se apilan verticalmente en pantallas pequeñas gracias al uso de `col-sm-3` y `col-sm-9`.

## Cómo verlo localmente

Simplemente abre el archivo `index.html` en cualquier navegador web moderno. No requiere instalación de dependencias, ya que Bootstrap y los íconos se cargan desde un CDN.

## Publicación (GitHub Pages)

1. Sube este proyecto a un repositorio público de GitHub.
2. Ve a **Settings > Pages** en el repositorio.
3. En **Source**, selecciona la rama `main` y la carpeta `/root`.
4. Guarda los cambios; GitHub te dará una URL pública donde estará publicada la página.
