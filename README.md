# Mi Rincón Deco — Landing de desechables

Landing page estática para **Comercializadora Mi Rincón Deco**: bolsas de basura, bolsas plásticas y de papel, vasos, platos, cubiertos y otros artículos desechables al por mayor.

- `index.html`: página completa (HTML + CSS + JS, sin dependencias).
- `img/`: fotos de los productos, recortadas del catálogo.

## Configuración

1. **WhatsApp**: en `index.html`, busca `const WHATSAPP = "";` y pon el número con código de país, sin `+` ni espacios (ej. `56912345678`).
2. **Precios y productos**: están en el arreglo `P` dentro de `index.html`. Cada producto tiene `id` (= nombre de la imagen en `img/`), categoría, nombre, descripción y sus presentaciones `[nombre, precio]`.

## Publicar

Al ser un sitio estático se puede publicar gratis con GitHub Pages (Settings → Pages → rama `main`, carpeta raíz), Netlify o Vercel.
