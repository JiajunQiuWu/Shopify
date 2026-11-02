# Compra con confianza

Sección de beneficios para fichas de producto Shopify, diseñada para presentar de forma clara la información que ayuda a comprar: envío, pago seguro y devoluciones. Se integra después del contenido principal del producto y permite adaptar los textos desde la configuración de la sección.

## Problema que resuelve

Las condiciones de envío, pago y devolución pueden quedar dispersas o pasar desapercibidas durante la compra. «Compra con confianza» las reúne en tarjetas breves y reconocibles, para que el cliente pueda consultar estos beneficios directamente en la ficha del producto.

## Funcionalidades implementadas

- Integración de la sección **Beneficios del producto** después de la sección principal en la plantilla de producto.
- Título de sección editable.
- Hasta 12 bloques de beneficio, cada uno con selección de icono, título y descripción.
- Tres opciones de icono SVG: envío, pago seguro y devoluciones.
- Tres beneficios de ejemplo incluidos en la plantilla y en el preset de la sección.
- Diseño responsive: tres columnas en escritorio, dos hasta 900 px y una hasta 600 px.
- Marcado accesible: nombre de sección configurable y los iconos decorativos excluidos de lectores de pantalla.
- Sin JavaScript ni dependencias externas.

## Tecnologías

- Shopify Liquid y esquema de secciones de Shopify.
- Plantilla JSON de producto.
- CSS encapsulado con `{% stylesheet %}`.
- SVG inline.

## Instalación

Duplica el tema antes de realizar cambios.

1. Copia [`product-benefits.liquid`](../../spectacular-focus-theme/sections/product-benefits.liquid) en la carpeta `sections/` del tema de destino.
2. En **Tienda online > Temas > Personalizar**, abre una plantilla de producto y añade **Beneficios del producto**.
3. Guarda los cambios y comprueba la página en escritorio y móvil.

La sección ya está incluida en la plantilla de referencia [`product.json`](../../spectacular-focus-theme/templates/product.json). Si se integra manualmente en otra plantilla JSON, añade una sección con `"type": "product-benefits"` y su clave correspondiente en el array `"order"`.

El tema de destino debe admitir secciones Liquid con bloques, plantillas JSON de producto y `{% stylesheet %}`. Si el tema usa otro sistema de layout o no define las variables `--color-background` y `--color-foreground`, puede ser necesario adaptar los estilos.

## Personalización

Desde el editor visual de Shopify:

1. Abre una plantilla de producto y selecciona **Beneficios del producto**.
2. Cambia el título de la sección.
3. En cada bloque **Beneficio**, selecciona **Envío**, **Pago seguro** o **Devoluciones** y edita el título y la descripción.
4. Añade, elimina o reordena bloques, hasta un máximo de 12.

Los valores iniciales también se pueden cambiar en la plantilla JSON del tema.

## Capturas

No hay capturas reales de escritorio ni de móvil en el repositorio, así que no se incluyen imágenes ni enlaces de captura pendientes que puedan parecer reales. Añade las capturas del tema cuando estén disponibles, por ejemplo, en `portfolio/product-benefits/screenshots/`.

## Pruebas y estado de verificación

- `shopify theme check`, ejecutado desde `spectacular-focus-theme`: **40 archivos inspeccionados, sin incidencias**.
- Se verificó en el código que la sección existe y que `product.json` la referencia después de la sección principal.
- El comportamiento responsive se ha comprobado visualmente.
- En la sesión actual no se han vuelto a verificar la edición ni el guardado de bloques desde el editor de temas de Shopify.
- No se ha comprobado la instalación en otros temas ni se ha publicado o desplegado el proyecto.

## Limitaciones conocidas

- Solo están disponibles los tres iconos incluidos; no se admiten iconos personalizados desde el editor.
- Título y descripción son texto plano, sin enlaces ni contenido enriquecido.
- Los puntos de cambio responsive (900 px y 600 px) están definidos en el CSS.
- Los colores dependen de las variables del tema compatible.
- Las capturas reales todavía no están disponibles en el repositorio.
