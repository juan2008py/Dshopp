# NIDESX — Tienda de ropa, calzados y accesorios

NIDESX es un catálogo en línea pensado para que encontrar y consultar productos sea sencillo. La tienda presenta prendas, calzados y accesorios con una experiencia clara, adaptable a móviles y enfocada en el contacto directo con Denis por WhatsApp.

## ¿Qué ofrece?

- **Catálogo dinámico:** carga los productos desde una hoja de cálculo pública de Google Sheets, por lo que la información puede actualizarse sin editar la página.
- **Información de cada producto:** muestra imagen, categoría, nombre, precio y estado, como disponible, pendiente o fuera de stock.
- **Consulta y pedido por WhatsApp:** cada producto incluye un botón que abre una conversación con un mensaje preparado con el nombre, la categoría y el precio del artículo.
- **Diseño adaptable:** la cuadrícula de productos y sus tarjetas se ajustan a pantallas pequeñas y grandes.
- **Estados de carga y mensajes informativos:** comunica cuando se está cargando el catálogo, cuando no hay productos y cuando ocurre un problema de conexión. Si una imagen no se puede cargar, se muestra una imagen alternativa.
- **Selección de productos:** el catálogo procesa las filas que tienen un identificador de producto válido.

## ¿Qué transmite?

La página transmite una propuesta cercana, práctica y accesible: una tienda personal que combina calidad con precios pensados para sus clientes. Su diseño limpio y directo pone los productos en primer plano y facilita pasar de descubrir un artículo a consultar por él, sin pasos innecesarios.

## Tecnologías

El proyecto está implementado en un único archivo `index.html` con **HTML, CSS y JavaScript**. JavaScript obtiene y presenta los datos publicados como CSV desde Google Sheets, y los enlaces de WhatsApp permiten contactar directamente con la tienda.

## Cómo funciona el catálogo

1. La página solicita los datos publicados de Google Sheets.
2. Lee el CSV y prepara las tarjetas de los productos con identificadores válidos.
3. Presenta la información y genera para cada producto un enlace de consulta por WhatsApp.

> El catálogo necesita conexión a Internet para cargar los datos y las imágenes externas. Si no se reciben productos, la página muestra un mensaje en lugar de las tarjetas.
