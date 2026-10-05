# Mi Rincón Deco — Landing de desechables

Landing page estática para **Comercializadora Mi Rincón Deco**: bolsas de basura, bolsas plásticas y de papel, vasos, platos, cubiertos y otros artículos desechables al por mayor.

- `index.html`: página completa (HTML + CSS + JS, sin dependencias).
- `img/`: fotos de los productos, recortadas del catálogo.

## Configuración

1. **WhatsApp**: configurado en `const WHATSAPP = "56988994814";` dentro de `index.html`. Para cambiarlo, usa el número con código de país, sin `+` ni espacios (ej. `56912345678`).
2. **Precios y productos**: están en el arreglo `P` dentro de `index.html`. Cada producto tiene `id` (= nombre de la imagen en `img/`), categoría, nombre, descripción y sus presentaciones `[nombre, precio]`.

3. **Registro de clientes**: el formulario "Registra tu negocio" pide nombre, WhatsApp, RUT de la empresa (con validación del dígito verificador), nombre del negocio, tipo de negocio y comuna.
   - Para guardar los registros en una base de datos, pon en `const REGISTRO_WEBHOOK = "";` la URL de un webhook. En GoHighLevel: Automatización → crear workflow → disparador **Inbound Webhook** → copiar la URL, y en el workflow mapear los campos (`nombre`, `whatsapp`, `rut`, `negocio`, `tipo_negocio`, `comuna`, `region`) a un contacto.
   - Mientras no haya webhook, el cliente envía sus datos por WhatsApp con un mensaje ya armado.

## Publicar

Al ser un sitio estático se puede publicar gratis con GitHub Pages (Settings → Pages → rama `main`, carpeta raíz), Netlify o Vercel.
