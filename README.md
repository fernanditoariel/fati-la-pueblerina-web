# Fati la Pueblerina — sitio web

Landing de la pastelería artesanal de Fátima Boscardín (Jacinto Aráuz / Bahía
Blanca, Argentina). HTML + CSS + JS estático, sin build.

## Ver local

```bash
python3 -m http.server 5178
```

Abrir `http://localhost:5178`.

## Assets

- **Fotos de producto**: 6 fotos reales tomadas del feed público de Instagram
  de `@lapueblerinasabores` (`assets/img/g-torta-*.jpg` y
  `hero-torta-chocolate.jpg`), redimensionadas y comprimidas con `sips`.
- **Logo**: el logo real (fondo rosa, ícono de gorro de chef, "Fati La
  Pueblerina Sabores Artesanales") no llegó como archivo descargable en la
  conversación, solo se vio en pantalla. Se recuperó la foto de perfil pública
  de Instagram (150×150) y se usa como ícono circular en el nav, footer y
  favicon/apple-touch-icon. El wordmark grande del nav/footer está tipeado en
  Alex Brush (script) para que coincida con el estilo del logo real.
- **og-cover.jpg**: armado a medida con Pillow (logo + tipografía), no con el
  script genérico de la skill (el logo no tiene fondo blanco/negro para keyar).

## Pendientes para Fernando / Fátima

- [ ] **Logo real en alta resolución**: pedirle a Fátima el archivo original
  del logo (PNG/AI/PSD) para reemplazar el wordmark tipográfico y el ícono de
  150px por el logo real en buena resolución.
- [ ] **Fotos propias en alta resolución**: las 6 fotos usadas vienen del feed
  público de Instagram (comprimidas a ~640px por Instagram). Si Fátima tiene
  las fotos originales en el rollo de cámara, reemplazarlas mejora bastante la
  nitidez en pantallas grandes.
- [ ] **Pan dulce navideño**: hay fotos en el Instagram pero con una plantilla
  de marca superpuesta (bordes rosas, no aptas para usar tal cual en la web).
  Se puede sumar como categoría de temporada más adelante con una foto limpia.
- [ ] **Confirmar el mensaje precargado de WhatsApp**: se armó un texto propio
  ("Hola Fati! Vi tu página web de La Pueblerina y quiero consultar por un
  pedido"). El bio de Instagram tiene uno parecido pero recortado en pantalla,
  confirmar si Fátima prefiere otro texto.
- [ ] **Dominio propio**: hoy el sitio vive en `*.vercel.app`. Si más adelante
  quieren un dominio propio, avisar antes de mover el alias de producción.

## Deploy

GitHub `fernanditoariel/fati-la-pueblerina-web` → Vercel team `coachfernando`,
auto-deploy en cada push a `main`.
