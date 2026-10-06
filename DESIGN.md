---
name: Temple
description: "El carácter se forja — sistema visual de la marca de rugby Temple"
colors:
  primary: "#6e2e24"
  primary-hi: "#8b1a1a"
  on-primary: "#faf9f6"
  base: "#faf9f6"
  surface: "#f0ede8"
  ink: "#141311"
  ink-dim: "#6a6560"
  line: "#ddd9d0"
  cream-warm: "#e8d5c4"
  night: "#0d0b09"
  footer-bg: "#141210"
  footer-ink: "#cfc9c2"
  footer-dim: "#8f8880"
  footer-line: "#302c28"
typography:
  display:
    fontFamily: "Archivo Black, system-ui, sans-serif"
    fontSize: "6rem"
    fontWeight: 400
    lineHeight: 0.88
    letterSpacing: "0"
  headline:
    fontFamily: "Archivo Black, system-ui, sans-serif"
    fontSize: "clamp(1.9rem, 4.2vw, 3rem)"
    fontWeight: 400
    lineHeight: 0.95
    letterSpacing: "-0.03em"
  title:
    fontFamily: "Archivo Black, system-ui, sans-serif"
    fontSize: "1.2rem"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "-0.02em"
  body:
    fontFamily: "Archivo, system-ui, -apple-system, Segoe UI, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "-0.01em"
  label:
    fontFamily: "Archivo Black, system-ui, sans-serif"
    fontSize: "0.78rem"
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: "0.09em"
rounded:
  cta: "7px"
  md: "8px"
  lg: "16px"
  mark: "9px"
  pill: "99px"
spacing:
  sm: "8px"
  md: "16px"
  lg: "28px"
  xl: "48px"
  section: "104px"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label}"
    rounded: "{rounded.md}"
    padding: "0.85rem 1.7rem"
  button-primary-hover:
    backgroundColor: "{colors.primary-hi}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label}"
    rounded: "{rounded.md}"
    padding: "0.85rem 1.7rem"
  button-cream:
    backgroundColor: "{colors.base}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.md}"
    padding: "0.85rem 1.7rem"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "#ffffff"
    typography: "{typography.label}"
    rounded: "{rounded.md}"
    padding: "0.85rem 1.7rem"
  button-sm:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.label}"
    rounded: "{rounded.md}"
    padding: "0.6rem 1.15rem"
  product-cta:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.cta}"
    padding: "0.55rem 1.1rem"
  card-media:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
---

# Design System: Temple

## Overview

**Creative North Star: "La Forja"**

Temple no vende ropa deportiva: forja carácter. El sistema se piensa como un taller — tierra cocida, óxido, cuero viejo y papel de estraza — no como una tienda online. La superficie base es crema cálida (papel, no blanco de galería), la tinta es casi negra, y un solo rojo profundo aparece como brasa: se enciende donde hay que actuar y se apaga en el resto. La profundidad se resuelve por capa tonal y por vidrio esmerilado, nunca por sombra difusa: nada flota, todo está apoyado.

La densidad es media con ritmo de editorial: bloques de sección generosos (104px) separados por bandas de superficie con filete, y dentro de cada bloque grillas auto-ajustadas que se reordenan sin saltos. La tipografía empuja hacia el extremo: Archivo Black en mayúsculas para todo lo que se navega, se acciona o se proclama; Archivo regular para todo lo que se lee. Entre esas dos posturas no hay término medio, y esa dureza es la personalidad.

La antireferencia está confirmada: **no Shopify genérico**. Nada de grillas suaves con badges de descuento, sombras de tarjeta a diez sombras, botones pill redondeados ni lenguaje de plantilla de e-commerce. Si una decisión se parece a un template de tienda, está mal hecha.

**Key Characteristics:**
- Papel crema + tinta casi negra + una sola brasa (`--accent`) que solo se enciende en acciones y en la banda manifiesto.
- Archivo Black en mayúsculas tracked para navegación, botones y precios; Archivo regular para prosa.
- Grillas `auto-fit` con `minmax` que nunca muestran huecos ni desbordan: 3 productos, 3 accesorios, 3 looks, footer de 4 columnas.
- Superficies planas; el único material "flotante" es la nav sticky en vidrio esmerilado.
- Movimiento preciso y con peso: `cubic-bezier(.16,1,.3,1)`, entradas con blur+rise, revelados por clip-path con stagger de 0.09s.

## Colors

Paleta de taller: papel, tinta y una brasa. Un solo acento cálido con contraste alto, sostenido por neutros crema que nunca llegan al blanco puro.

### Primary
- **Óxido de Forja** (`#6e2e24`): el acento de la marca. Botones sólidos, precios de accesorios, nav activa, foco, selección de texto y la banda manifiesto. Es tierra cocida, no rojo de oferta.
- **Óxido Encendido** (`#8b1a1a`): estado hover del acento. Solo aparece bajo el cursor, nunca en reposo.
- **Sobre Brasa** (`#faf9f6`): texto sobre el acento; es el papel base devuelto como tinta invertida.

### Neutral
- **Papel** (`#faf9f6`): fondo base de la página en tema claro. No es blanco.
- **Papel Sombra** (`#f0ede8`): bandas de superficie (`band-surface`) y fondo de los media en carga.
- **Tinta** (`#141311`): texto de cuerpo y titulares; también el fondo de la página en tema oscuro.
- **Tinta Apagada** (`#6a6560`): descripciones, lead de contacto, texto legal del footer.
- **Filete** (`#ddd9d0`): bordes de sección, subrayados de enlace de contacto, separadores.

### Supporting
- **Crema Cálido** (`#e8d5c4`): tagline del hero y hover del botón crema. El único tono "cálido claro" del sistema.
- **Noche** (`#0d0b09`): fondo de la placa del hero y de toda la superficie oscura del primer viewport.
- **Footer** (`#141210` / `#cfc9c2` / `#8f8880` / `#302c28`): el bloque final es un mundo aparte, más oscuro que cualquier otra superficie, con filete propio.

### Dark Theme
El tema oscuro no es una inversión: es el mismo sistema con la brasa prendida. `--base` pasa a `--ink` (`#141311`), la tinta a `#f5f3ef`, y el acento se enciende a `#dd8873` con hover `#f0a491` y sobre-brasa `#17130f`. Los roles no cambian, solo la temperatura.

### Named Rules
**The Ember Band Rule.** El acento inunda exactamente una banda a todo el ancho del sitio: el manifiesto "Diseñado para el rugby, hecho para durar". En cualquier otro lugar es una chispa —botón, precio, nav activa, anillo de foco, `::selection`— y jamás un fondo de tarjeta ni un color de texto corrido.

**The Night Rule.** `--night` es la superficie más oscura del sistema y está reservada al hero. Ninguna otra sección baja a ese valor: si algo que no es el primer viewport se pone tan oscuro como la noche, compite con el hero.

## Typography

**Display Font:** Archivo Black (con `system-ui, sans-serif` como fallback)
**Body Font:** Archivo 400/500/600/700 (con `system-ui, -apple-system, 'Segoe UI', sans-serif`)

**Character:** Una sola familia en dos pesos extremos. Archivo Black grita en mayúsculas comprimidas (`-0.03em`) todo lo que se navega o se proclama; Archivo regular fluye en prosa con tracking sutil (`-0.01em`). El pareamiento es monolítico a propósito: no hay serif de contraste, no hay tercera voz.

### Hierarchy
- **Display** (400, `6rem`, line-height `.88`): el wordmark TEMPLE del hero, una letra por `<span>`, distribuido a todo el ancho con `justify-content:space-between`.
- **Headline** (400, `clamp(1.9rem,4.2vw,3rem)`, line-height `.95`): títulos de sección. En la banda manifiesto sube a `3.25rem` con line-height `1.05` y máximo `24ch`.
- **Title** (400, `1.2rem`, letter-spacing `-.02em`): nombres de producto, accessory, look y figcaption. Los del footer bajan a `.75rem` en mayúsculas con tracking `.13em`.
- **Body** (400, `1rem`, line-height `1.5`): prosa, con anchos máximos declarados para no pasarse —`54ch` en el lede del hero, `34ch` en descripciones de producto, `36ch` en captions, `38ch` en el párrafo de footer.
- **Label** (400, `.78rem`, letter-spacing `.09em`, uppercase): nav (`.74rem`/`.11em`), botones (`.78rem`/`.09em`, sm `.72rem`/`.1em`, lg `.84rem`), CTA de producto (`.72rem`/`.1em`), marca de nav (`.95rem`/`.16em`).

### Named Rules
**The Uppercase Rule.** Todo lo que el visitante puede tocar o por donde puede moverse va en Archivo Black mayúsculas con tracking entre `.09em` y `.16em`: nav, botones, CTA, títulos de footer, marca. La prosa jamás se pone en mayúsculas, y un título de sección jamás se pone en minúsculas.

**The Full-Width Wordmark Rule.** TEMPLE siempre ocupa el 100% del contenedor, letra por letra separada, sin reordenar ni escalerar según el contenido. El tamaño solo baja por breakpoint: `6rem` → `4.75rem` (≤1100px) → `3.5rem` (≤700px).

## Layout

Contenedor único: `.wrap` con `max-width:1200px`, centrado, `padding-inline:2rem` (`1.25rem` bajo 640px). Todo —nav, hero, secciones, footer— pasa por ese contenedor; el ancho de lectura se controla después con `max-width` en ch.

Ritmo vertical de secciones: `6.5rem` (104px) en desktop, `5rem` (80px) bajo 900px, `3.75rem` (60px) bajo 640px. La banda manifiesto mantiene su propio pulso (`4.5rem` / `3rem`). El `section-head` separa del contenido con `3rem` (`2rem` en mobile).

Grillas por `repeat(auto-fit,minmax(min(100%,N),1fr))` — nunca columnas fijas:
- **Productos:** `min(100%,258px)`, gap `clamp(1.75rem,3vw,2.5rem)`, media en `aspect-ratio:4/5`.
- **Accesorios:** columna única (`1fr`) de filas a todo el ancho, cada una en `176px minmax(0,1fr) auto` con media cuadrada de `176px` (`96px` bajo 640px), filete de 1px `--line` entre filas, padding `1.75rem 1rem` y `margin-inline:-1rem` para que el hover pinte hasta el borde del contenedor. El precio va alineado a la derecha (izquierda, bajo la descripción, en mobile).
- **Lookbook:** `min(100%,290px)`, gap `clamp(1.75rem,3vw,2.5rem)`, media en `3/4`.
- **Footer:** `min(100%,210px)`, gap `clamp(2rem,4vw,3rem)`.
- **Contacto:** excepción con columnas explícitas `1.45fr 1fr`, gap `clamp(2.5rem,6vw,5rem)`; colapsa a una sola columna bajo 860px.

Hero: `min-height:92svh` con la placa absoluta detrás y el copy anclado abajo (`align-items:flex-end`). Bajo 860px el hero se apila —placa arriba en `4/3`, copy abajo sobre fondo sólido— y desaparece el degradado de legibilidad: no se pone scrim sobre texto.

Breakpoints observados: `1100px` (wordmark), `900px` (ritmo y banda), `860px` (contacto + hero apilado), `700px` (wordmark chico), `640px` (mobile: gutters, nav sin links, ritmo).

## Elevation & Depth

El sistema es plano: no hay sombras de tarjeta, ni bordes inferiores de tarjeta, ni elevación en reposo. La profundidad se resuelve de dos formas —capa tonal y material— y ninguna usa `box-shadow` como lenguaje. La única sombra del sitio es el sello de la nav (`0 2px 6px -2px rgba(20,19,17,.45)`), un aterrizaje mínimo para que la marca no se pegue al vidrio.

### Shadow Vocabulary
- **Sello de marca** (`box-shadow: 0 2px 6px -2px rgba(20,19,17,.45)`): únicamente sobre `img.nav-mark`, para separar el logo del fondo vidrio.

### Named Rules
**The Glass Rule.** La nav sticky es el único material translúcido del sistema: `rgba(250,249,246,.88)` en tema claro / `rgba(20,19,17,.88)` en oscuro, con `backdrop-filter:saturate(150%) blur(14px)` y filete inferior de 1px. Si otro elemento quiere vidrio, le falta una razón.

**The Tonal Layer Rule.** La jerarquía de planos se lee por color, no por sombra: `--surface` con filete separa bloques, `--base` deja respirar, el footer cierra. Los alternados `band-surface` son el mecanismo de ritmo, no decoración.

## Shapes

Lenguaje de esquina suave pero contenido: **16px** es la medida de toda media y tarjeta (`.media`, `.product`), que es lo que hace que las fotos se sientan apoyadas y no recortadas a cuchillo. Los controles bajan a **8px** (`.btn`), los CTA internos a **7px** (`.product-cta`, `.skip`) y el sello de marca queda en **9px**. No hay ningún elemento con `border-radius:50%` ni pill completo en todo el sistema, salvo el thumb del scrollbar (`99px`).

Bordes: **1.5px** para los controles accionables (`.btn`, `.product-cta`), **1px** para separadores estructurales (nav, `band-surface`, footer legal, enlaces de contacto), **2px** para el indicador de nav activa. El foco es **2px** sólido con offset **3px** (`#fff` dentro del hero, acento en el resto) y radio **3px**.

## Components

### Buttons
- **Shape:** esquinas de 8px (`rounded.md`), borde de 1.5px, padding `0.85rem 1.7rem`; variantes sm `0.6rem 1.15rem` (`.72rem`) y lg `1.05rem 2.3rem` (`.84rem`).
- **Primary (`.btn-solid`):** fondo Óxido de Forja, texto sobre brasa, hover enciende a `#8b1a1a`.
- **Cream (`.btn-cream`):** papel sobre tinta, hover cae a Crema Cálido `#e8d5c4`. Solo existe sobre superficie oscura (hero).
- **Ghost (`.btn-ghost`):** transparente con borde blanco al 55%, hover rellena blanco al 14% y completa el borde. También, solo, sobre superficie oscura.
- **Hover / Focus:** todo botón sube `translateY(-2px)` en `.15s` y vuelve a `0` en `:active`; los colores transicionan en `.2s`. Foco visible con anillo de 2px.
- **Todas las variantes** comparten tipografía Label en mayúsculas.

### Product CTA (chip de compra)
- **Shape:** borde 1.5px tinta, esquina 7px, padding `0.55rem 1.1rem`.
- **State:** en reposo es outline; al hover o al `:focus-visible` de la tarjeta se llena de acento con texto sobre brasa. Nunca tiene fondo propio en reposo — es la única "acción" que espera a que mires la tarjeta.

### Cards / Containers
- **Corner Style:** 16px en media y en el contenedor del producto.
- **Background:** el media hereda `--surface`; el cuerpo de la tarjeta es transparente sobre la superficie de la sección.
- **Shadow Strategy:** ninguna. Separación por `gap` de `clamp(1.75rem,3vw,2.5rem)`.
- **Internal Padding:** el cuerpo baja `1.15rem` del media y apila con `gap:.6rem`; el precio empuja el CTA al fondo con `margin-top:auto`.
- **Hover:** la imagen escala a `1.05` en `.6s` con la misma curva de entrada; el chip de compra se enciende.

### Navigation
- **Style:** sticky `top:0`, alto `4rem` (`3.5rem` mobile), vidrio esmerilado, filete inferior 1px.
- **Typography:** marca en Label a `.95rem`/`.16em` con sello de 34px; links en Label a `.74rem`/`.11em` con subrayado inferior de 2px transparente.
- **Active:** el link de la sección en vista gana `color:var(--accent)` y `border-bottom-color` de 2px, sincronizado por IntersectionObserver con `rootMargin:-45% 0 -50% 0`.
- **Mobile:** bajo 640px los links desaparecen y queda marca + botón "Pedir".

### Accessory Row
- **Shape:** fila a todo el ancho, esquinas 16px, padding `1.75rem 1rem` con `margin-inline:-1rem`; media cuadrada de 176px (96px bajo 640px) con el mismo reveal clip-path que el resto.
- **Structure:** tres columnas `media | cuerpo | precio`; entre filas, un filete de 1px `--line`. Nunca es tarjeta: es una lista de precios.
- **Typography:** título en Title (1.2rem), descripción en Body con máximo `34ch`, precio en 700 con `tabular-nums` y color acento, alineado a la derecha.
- **Hover / Focus:** el fondo sube a `--base`, la imagen escala a `1.05` y el foco mantiene offset 4px.

### Manifesto Band
Bloque a todo el ancho, fondo acento, texto sobre brasa, `4.5rem` de padding, declaración a `3.25rem` con máximo `24ch`. Es el único lugar donde el acento ocupa fondo completo.

### Hero
Placa fotográfica a `92svh` con degradado nocturno (`rgba(13,11,9,.14)` → `.94`), wordmark blanco a todo el ancho, tagline en Crema Cálido y lede en `#e3ddd7`. Botón crema sólido + botón ghost en la fila de acciones.

### Lookbook Figure
Media `3/4` con reveal, `figcaption` a `1.1rem` del media, título en Title y párrafo en `--ink-dim` con máximo `36ch`. Sin overlay ni caption encima de la imagen.

### Signature: el revelado
Todo media entra con `clip-path: inset(0 0 100% 0)` → `inset(0 0 0 0)` en `.8s`, con stagger de `.09s` por posición en la grilla (1°/2°/3°). El clip-path vive en el `<img>`, nunca en el elemento observado — moverlo rompe el `IntersectionObserver`. El hero, en cambio, entra con `letterRise` (blur 9px → 0 + rise `.38em`) escalonado `.06s` por letra.

## Do's and Don'ts

### Do:
- **Do** resolver jerarquía con capa tonal (`--surface` + filete) antes que con sombra; la única sombra permitida es la del sello de nav.
- **Do** mantener los anchos de lectura declarados: `54ch` lede, `34ch` descripción de producto, `36ch` caption, `38ch` footer.
- **Do** usar las grillas `auto-fit` con `minmax` y `min(100%,N)` para que nunca aparezca un hueco ni desborde en tablet.
- **Do** dejar que el acento inunde solo la banda manifiesto; en el resto es botón, precio, nav activa o foco.
- **Do** respetar `prefers-reduced-motion`: el sistema ya anula animaciones y transiciones, no reintroducir movimiento condicional sin esa guarda.
- **Do** dar foco visible a todo lo accionable: 2px sólido, offset 3px, `#fff` sobre el hero.

### Don't:
- **Don't** usar el acento como fondo de tarjeta, de sección o de texto corrido fuera de la banda manifiesto.
- **Don't** añadir sombras de tarjeta, elevación en reposo ni `border-radius:50%` / pill: no existen en este sistema.
- **Don't** pasar los titulares de sección a Archivo regular ni bajar los labels de mayúsculas.
- **Don't** poner scrim sobre texto en mobile: el hero apilado usa fondo sólido, no degradado encima de la copia.
- **Don't** mover el `clip-path` del `<img>` al contenedor `.reveal`: el elemento deja de ser observable y el media queda invisible.
- **Don't** acercarse a un template de tienda (anti-referencia confirmada): sin badges de descuento, sin grilla de "ofertas", sin botones pill.
