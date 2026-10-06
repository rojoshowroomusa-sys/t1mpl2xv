# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

El jugador de rugby es el eje: hombre 18-40, socio o jugador de clubes de Argentina, que entra a la web desde el celular, muchas veces después del entrenamiento o del partido, y termina escribiendo por WhatsApp.

Su entorno —familia, pareja, amigos— es la segunda audiencia: compra sobre todo accesorios (cuadro, cartas, taza) y prendas para regalar, a partir del vínculo con ese jugador.

## Product Purpose

Temple vende ropa y objetos de rugby: Polo, Hoodie y Campera, más Cuadro, Cartas y Taza. Existe para que alguien que se reconoce en la mentalidad del rugbier pueda llevarse esa actitud puesta y hacerla visible en el club.

El éxito es una conversación: la web cumple su función cuando alguien aprieta y abre el chat de WhatsApp con una compra empezada.

## Positioning

Marca propia de club y comunidad. Temple no vende una prenda técnica, vende el pertenecer al grupo y al club: el after, el de al lado, levantarse después del tackle. Una vecina puede copiar una frase o un corte, no puede copiar el vínculo de comunidad sobre el que se apoya la marca.

## Operating Context

- Los pedidos se cierran en WhatsApp, en el celular, en conversación directa.
- Canales confirmados: WhatsApp (`wa.me`), Instagram `@temple.argentina`, email `hola@temple.art`.
- Desplegada en Cloudflare Pages en `https://t1mpl2xv.pages.dev/`.
- Contexto de uso real: club, entrenamiento, partido, after. El sitio se lee en horarios de ocio, no en contexto de oficina.

## Capabilities and Constraints

- **Compra solo por WhatsApp.** No hay carrito, ni checkout, ni pagos online. Cualquier trabajo futuro debe preservar ese camino.
- **Precios reales en pesos argentinos** (confirmados vigentes): Polo $89.000 · Hoodie $124.000 · Campera $168.000 · Cuadro $42.000 · Cartas $12.000 · Taza $18.000.
- **Idioma es_AR**, escrito en voseo.
- Sitio estático de una sola página (HTML/CSS/JS sin build ni backend) servido desde Cloudflare Pages, con assets locales en `v2/images/`.
- Sin información de talles, envíos ni devoluciones en el sitio: es un hecho abierto, no una promesa que el sitio pueda hacer.

## Brand Commitments

- Nombre: **Temple**. Tagline: **"El carácter se forja"**. Frase de marca: **"Diseñado para el rugby, hecho para durar."**
- Voz: voseo argentino y tono directo, confirmado como innegociable en todo el copy.
- Activo de marca: `v2/images/temple-mark.png` (sello) y `v2/images/temple-og-1200.jpg` (imagen de compartir).
- Assets de producto propios: fotos/render de Polo, Hoodie y Campera (`temple-{polo,hoodie,campera}-{560,840,1200}.png`), accesorios (`temple-{cuadro,cartas,taza}.png`), hero `temple-xv-hero-{768,1152,1536}.jpg`.

## Evidence on Hand

- Copy completo y real en `v2/index.html`: hero, colección, accesorios, lookbook, contacto, footer.
- Imágenes propias de producto y hero en `v2/images/` (listadas arriba).
- Ausencias que future work no debe inventar: no hay testimonios, ni prensa, ni clientes citados, ni fotos reales de personas usando la prenda (el lookbook usa fotos de stock de Unsplash), ni datos de envío/pago/talles.

## Product Principles

1. **El pedido es una conversación.** La web existe para abrir el chat de WhatsApp, no para cerrar la venta sola.
2. **El jugador manda, el entorno acompaña.** Se diseña pensando en quien juega; quien lo rodea compra desde ese vínculo.
3. **La marca es un código, no una ficha técnica.** El mensaje, el grupo y la actitud pesan más que la descripción del tejido.
4. **Voz propia, sin corporativismo.** Frases cortas, voseo, cero lenguaje de e-commerce genérico.
5. **Nada inventado.** Precios, datos y promesas reales; ante la duda, se omite antes que se fabrica.
