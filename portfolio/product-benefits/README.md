# Product Benefits para Shopify

Sección reutilizable de beneficios para la ficha de producto de una tienda Shopify. Presenta cada beneficio como una tarjeta con icono, título y descripción, para que la tienda pueda comunicar información de compra relevante junto al producto.

## Problema que resuelve

La información sobre envíos, pagos y devoluciones puede quedar dispersa o pasar desapercibida en una ficha de producto. Esta sección la agrupa en un bloque visual, fácil de localizar y editable desde el personalizador del tema, sin tener que modificar el contenido Liquid para cada cambio.

## Funcionalidades

- Muestra un título de sección configurable.
- Permite añadir hasta 12 bloques de beneficio.
- Cada bloque tiene un icono seleccionable, un título y una descripción.
- Incluye tres iconos SVG: envío, pago seguro y devoluciones.
- Ofrece tres beneficios de ejemplo como contenido inicial.
- Adapta la cuadrícula al ancho de pantalla: tres columnas en escritorio, dos hasta 900 px y una hasta 600 px.
- Incluye etiquetas accesibles para la sección y marca los iconos como decorativos.

## Tecnologías

- Shopify Liquid y el esquema de sección de Shopify.
- Plantilla de producto JSON.
- CSS incluido en la sección mediante `{% stylesheet %}`.
- SVG inline para los iconos.

No requiere bibliotecas JavaScript ni dependencias externas.

## Instalación en un tema compatible

La sección está preparada para un tema Shopify que admita secciones Liquid con bloques y plantillas JSON de producto. El tema de este proyecto ya incluye la integración.

1. Duplica el tema de destino antes de modificarlo.
2. Copia [`product-benefits.liquid`](../../spectacular-focus-theme/sections/product-benefits.liquid) a la carpeta `sections/` del tema.
3. En el editor visual de Shopify, abre una plantilla de producto y añade la sección **Beneficios del producto**. Shopify actualizará la plantilla JSON correspondiente.
4. Si gestionas la plantilla manualmente, registra el tipo `product-benefits` en la plantilla JSON de producto y asigna el orden deseado. Puedes consultar la integración de este proyecto en [`product.json`](../../spectacular-focus-theme/templates/product.json).
5. Guarda y previsualiza el tema duplicado antes de publicarlo.

Comprueba que el tema de destino admite las etiquetas Liquid y el formato de plantilla utilizados por la sección.

## Personalización desde el editor visual

1. En Shopify, ve a **Tienda online > Temas > Personalizar**.
2. Abre una plantilla de producto, por ejemplo, **Producto predeterminado**.
3. Selecciona **Beneficios del producto** en la lista de secciones. Si aún no está en la plantilla, añádela desde el editor.
4. Edita el título de la sección.
5. En cada bloque **Beneficio**, selecciona uno de los tres iconos disponibles y cambia el título y la descripción.
6. Añade, elimina o reordena bloques según el contenido de la tienda, hasta el máximo de 12.
7. Guarda los cambios y revisa la vista previa en escritorio y móvil.

## Comprobaciones y limitaciones

- La sección está integrada en la plantilla de producto del proyecto y aparece después de la sección principal.
- El esquema limita la sección a 12 bloques y ofrece las opciones de icono **Envío**, **Pago seguro** y **Devoluciones**.
- La sección fue creada y probada en Shopify, según el estado indicado para este proyecto. Al preparar este README, se contrastó la implementación con los archivos fuente; no se ejecutaron pruebas adicionales ni se validó la instalación en otro tema.
- El contenido de los bloques es texto plano: no hay campos para enlaces, contenido enriquecido ni iconos personalizados desde el editor.
- Los puntos de cambio de columnas están definidos en el CSS de la sección (900 px y 600 px). No hay controles visuales para cambiar el diseño o esos valores.

## Capturas

Añade las imágenes en `portfolio/product-benefits/screenshots/` y actualiza las rutas si usas otros nombres.

### Escritorio

![Captura de la sección en escritorio — pendiente de añadir](./screenshots/escritorio.png)

### Móvil

![Captura de la sección en móvil — pendiente de añadir](./screenshots/movil.png)

### Editor de Shopify

![Captura de la sección en el editor visual de Shopify — pendiente de añadir](./screenshots/editor-shopify.png)
