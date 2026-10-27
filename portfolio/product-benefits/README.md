# Product Benefits para Shopify

Sección reutilizable para destacar beneficios de compra en la ficha de producto de una tienda Shopify. Presenta tarjetas con icono, título y descripción, integrada en la plantilla de producto del tema `spectacular-focus-theme`.

## Problema que resuelve

La información sobre envíos, pagos y devoluciones puede quedar dispersa o pasar desapercibida en una página de producto. Esta sección la reúne en un bloque visual situado después del contenido principal, para facilitar su consulta y permitir que el equipo de la tienda actualice los textos desde el editor visual de Shopify.

## Implementación realizada

- Se creó la sección Liquid [`product-benefits.liquid`](../../spectacular-focus-theme/sections/product-benefits.liquid).
- Se integró en la plantilla [`product.json`](../../spectacular-focus-theme/templates/product.json) después de la sección principal del producto.
- Se configuró el esquema de Shopify para editar el título y añadir hasta 12 bloques.
- Cada bloque permite seleccionar un icono, editar un título y añadir una descripción.
- Se añadieron tres bloques iniciales: envío rápido, pago seguro y devoluciones sencillas.
- Se incorporó diseño responsive: tres columnas en escritorio, dos hasta 900 px y una hasta 600 px.
- Se incluyeron iconos SVG inline para envío, pago seguro y devoluciones.
- Se añadieron etiquetas accesibles para la sección y se marcaron los iconos como decorativos.
- No se utilizan JavaScript ni dependencias externas.

## Tecnologías utilizadas

- Shopify Liquid.
- Esquema JSON de secciones de Shopify (`{% schema %}`).
- Plantilla JSON de producto.
- CSS incluido en la sección mediante `{% stylesheet %}`.
- SVG inline.

## Instalación en un tema Shopify compatible

Duplica el tema de destino antes de realizar cambios.

1. Copia [`product-benefits.liquid`](../../spectacular-focus-theme/sections/product-benefits.liquid) en la carpeta `sections/` del tema.
2. Abre **Tienda online > Temas > Personalizar**.
3. Abre una plantilla de producto y añade la sección **Beneficios del producto**.
4. Guarda y revisa la vista previa en escritorio y móvil.
5. Si gestionas la plantilla manualmente, añade una sección con el tipo `product-benefits` en el JSON de producto y colócala en el orden deseado. Consulta la integración de referencia en [`product.json`](../../spectacular-focus-theme/templates/product.json).

El tema compatible debe admitir secciones Liquid con bloques, plantillas JSON de producto y la etiqueta `{% stylesheet %}`. En otro tema podrían ser necesarios ajustes de layout o de las variables de color `--color-background` y `--color-foreground`.

## Personalización desde el editor visual

1. Ve a **Tienda online > Temas > Personalizar**.
2. Abre una plantilla de producto, como **Producto predeterminado**.
3. Selecciona **Beneficios del producto** o añádela si todavía no está en la plantilla.
4. Edita el título de la sección.
5. En cada bloque **Beneficio**, selecciona **Envío**, **Pago seguro** o **Devoluciones**.
6. Cambia el título y la descripción del bloque.
7. Añade, elimina o reordena bloques hasta un máximo de 12.
8. Guarda y revisa ambas vistas, escritorio y móvil.

## Comprobaciones realizadas y limitaciones

### Comprobaciones

- La sección está registrada en la plantilla de producto con el tipo `product-benefits`.
- La plantilla coloca la sección después de la sección principal.
- El esquema incluye el título, los bloques, las opciones de icono, el límite de 12 bloques y un preset con tres beneficios.
- Según el estado indicado para el proyecto, la funcionalidad fue creada y probada en Shopify.
- Para actualizar este README se contrastó la documentación con los archivos Liquid y JSON reales. No se ejecutaron pruebas adicionales ni se validó la instalación en otro tema.

### Limitaciones

- Solo hay tres iconos disponibles; no se pueden cargar iconos personalizados desde el editor.
- Los campos de título y descripción son texto plano, sin enlaces ni contenido enriquecido.
- Los puntos de cambio responsive están definidos en el código: 900 px y 600 px.
- Los colores dependen de las variables del tema compatible.
- Este documento no incluye publicación, despliegue ni configuración de una tienda.

## Capturas

Sustituye las imágenes pendientes por capturas reales. Se propone guardarlas en `portfolio/product-benefits/screenshots/`.

### Escritorio

![Captura de Product Benefits en escritorio — pendiente de añadir](./screenshots/escritorio.png)

### Móvil

![Captura de Product Benefits en móvil — pendiente de añadir](./screenshots/movil.png)

### Editor de Shopify

![Captura de Product Benefits en el editor visual de Shopify — pendiente de añadir](./screenshots/editor-shopify.png)
