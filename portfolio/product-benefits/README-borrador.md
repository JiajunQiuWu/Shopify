# Product Benefits — Sección personalizable para Shopify

Sección reutilizable para páginas de producto de Shopify que permite mostrar ventajas de compra de forma clara y adaptable a diferentes dispositivos.

## Objetivo

Ayudar a una tienda online a comunicar información útil —como envíos, pagos y devoluciones— cerca de la ficha de producto, sin necesidad de editar código cada vez que cambie el contenido.

## Funcionalidades

- Tres beneficios iniciales: **Envío rápido**, **Pago seguro** y **Devoluciones sencillas**.
- Títulos y descripciones editables desde el editor visual de Shopify.
- Bloques que se pueden añadir, eliminar y reordenar.
- Distribución responsive: tres columnas en escritorio y una en móvil.
- Estilos encapsulados para reducir conflictos con otras secciones del tema.
- Integración en la plantilla de producto predeterminada.

## Tecnologías

Shopify Liquid · JSON (schema y plantilla) · HTML · CSS · Shopify CLI · GitHub Copilot (asistencia al desarrollo).

## Archivos del proyecto

```text
sections/product-benefits.liquid
templates/product.json
```

El segundo archivo contiene la integración de la sección en la plantilla de producto. Si se reutiliza en otro tema, **no debe sustituirse por completo** su `templates/product.json`: hay que integrar la sección conservando la configuración existente.

## Instalación en otro tema

1. Haz una copia de seguridad o duplica el tema de destino.
2. Copia `sections/product-benefits.liquid` a la carpeta `sections/` del tema.
3. Abre el editor visual de Shopify y, en la plantilla de producto, busca y añade la sección de beneficios si está disponible como sección añadible.
4. Configura los bloques, títulos y descripciones.
5. Si se requiere que aparezca por defecto, integra su referencia en `templates/product.json` respetando el resto de las secciones y el orden existente.
6. Revisa el resultado en escritorio y móvil antes de publicar.

> La compatibilidad con otros temas debe comprobarse individualmente. Estas instrucciones describen el procedimiento general y no sustituyen una prueba de integración.

## Personalización

Desde el editor visual del tema, entra en **Productos → Producto predeterminado**, selecciona la sección de beneficios y edita los títulos y descripciones. También puedes añadir, eliminar o cambiar el orden de los bloques.

## Validación

- `shopify theme check`: según el resultado informado, 40 archivos inspeccionados y ningún error.
- Validación de `templates/product.json` y `git diff --check`: sin incidencias, según el resultado informado.
- Comprobación manual: la sección aparece en Shopify y permite editar los beneficios.
- **Pendiente de documentar con capturas:** presentación en escritorio, vista móvil y editor visual.

No se han medido mejoras en conversión o ventas. La sección es una mejora de presentación y editabilidad, no una garantía de resultados comerciales.

## Capturas

Añade aquí imágenes reales de tu tienda de pruebas:

### Escritorio

_Pendiente: `screenshots/desktop.png`_

### Móvil

_Pendiente: `screenshots/mobile.png`_

### Editor de Shopify

_Pendiente: `screenshots/editor.png`_

## Estado

Primera versión funcional, probada manualmente en una tienda Shopify de desarrollo. Proyecto de demostración para portfolio freelance; no es un producto comercial ni se ha validado en múltiples temas.
