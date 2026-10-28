# Casa de la Ribera II — Propiedad única

Proyecto de Propietas Inmobiliaria. Hereda de `../CLAUDE.md`: datos de la firma, manual de marca y reglas generales. Acá solo lo específico.

## El proyecto
- **Qué es:** casa en Playa Unión, comercializada en alquiler y venta. Fuente de los datos: listado en ipropietas.com.ar (publicado como "Zabala 331", sin descripción ni comodidades cargadas).
- **Ubicación:** Zabala 331, Playa Unión (Rawson, Chubut)
- **Oferta:** casa de 3 ambientes, 2 dormitorios, 2 baños, 74 m² totales, 5 años de antigüedad.
  - Alquiler: ARS 680.000 mensual (según listado; validar vigencia antes de publicar)
  - Venta: PENDIENTE (precio)
- **Estado:** disponible (según listado; confirmar)
- **Contacto específico:** usa el WhatsApp de la firma (`https://wa.me/5492804503151`)

## Identidad
- **Marca propia del desarrollo:** no. Usa solo Propietas (azul `#2e3092` / celeste `#27aae1`, Montserrat).
- **Rol de Propietas:** comercializadora (logo en header/footer + pie legal)
- **Paleta / tipografía:** la de la firma; ver DESIGN.md cuando exista

## Técnico
- **Stack:** delegado (HTML/CSS estático + JS mínimo, salvo que impeccable shape indique otra cosa)
- **Assets:** `assets/logos/` (color, blanco, símbolo) y `assets/img/foto-01..11.jpeg` (descargadas del listado, sin optimizar ni con `alt` definido)
- **Deploy:** PENDIENTE — publicar solo con confirmación del usuario

## Contexto de diseño
- `PRODUCT.md` (impeccable init) y `DESIGN.md` (cuando exista) son la fuente de verdad visual y de producto.

## Estado
- `index.html` construido (dirección "tabla de mareas", ver `.impeccable/surfaces/index-html.md`). Sin deploy. Falta: revisión en celular real, finish review, DESIGN.md.
- La calle no figura en la página: el listado dice Zabala 331 pero la foto-05 (no usada) muestra el número 327.
- Sin afirmar cercanía al mar: ninguna foto muestra el mar.

## Pendientes
- Precio de venta
- Descripción, comodidades, superficie cubierta/lote, orientación, cochera, mascotas
- Confirmar nombre público "Casa de la Ribera II" vs. dirección "Zabala 331" y si se muestra la dirección exacta
- Orden y descripción de las 11 fotos (para `alt` y jerarquía); ver si hay planos
- Condiciones de alquiler (contrato, garantía, expensas): no inventar
- Validar el pie legal con el corredor
