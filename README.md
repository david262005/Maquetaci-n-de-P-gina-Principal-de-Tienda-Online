# Tienda Online - Proyecto Bootstrap + Fetch API

**Diseñado por:** Anthony David Martínez León
**Carné:** 1890-23-23782

## Descripción del proyecto

Página web que simula una tienda en línea, construida con **HTML5**, **Bootstrap 5.3** y **JavaScript (Fetch API)**. El proyecto incluye un encabezado con carrusel de imágenes, un ícono de carrito de compras con contador dinámico, un menú de categorías y una sección de productos cargados de forma dinámica desde un backend (API REST) usando `fetch()` y `async/await`.

## Funcionalidad dinámica (Fetch API)

- Los productos ya no están escritos en el HTML: se obtienen desde el endpoint
  `https://backservicetest-g8emcvdff0fqe2b8.canadacentral-01.azurewebsites.net/api/producto`
- Se usa `fetch()` con `async/await` dentro de un bloque `try/catch` para manejar errores de conexión.
- Cada producto se recorre con `.forEach()` y se genera dinámicamente con `innerHTML` dentro de un `div` con `id="contenedor-productos"`.
- Si el producto tiene `enOferta == true`, se muestra el `precioOferta` junto al precio original tachado.
- Cada producto se coloca en un `div class="col-sm-12 col-md-4 mb-4"` para que se vea 1 por fila en móvil y 3 por fila en pantallas medianas/grandes.
- El botón "Agregar al carrito" de cada producto incrementa el contador visual del carrito en el navbar.

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