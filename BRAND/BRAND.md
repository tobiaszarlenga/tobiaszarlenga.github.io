# TobDev — sistema de logo

El símbolo (boina + anteojos) está **vectorizado del PNG original que pasaste**, sin redibujar.
Solo se generaron variantes de color y los lockups con el wordmark.

## Paleta

| Rol | HEX | Uso |
|-----|-----|-----|
| Navy marca | `#122A4D` | logo sobre fondo claro |
| Tinta mono | `#06172F` | impresión a 1 tinta / sellos |
| Violeta (gradient ini) | `#5B6FE4` | inicio del degradé |
| Cyan (gradient fin) | `#11BFD6` | fin del degradé |
| Blanco | `#FFFFFF` | logo sobre fondo oscuro |
| Fondo oscuro | `#0A0E1A` | fondo del sitio / avatares |

Degradé (igual que el hero del sitio):
```css
background: linear-gradient(135deg, #5B6FE4 0%, #11BFD6 100%);
```

## Qué archivo usar

- **Sitio (header, fondo oscuro):** `mark-white.svg` o `mark-gradient.svg`; lockup `lockup-horizontal-dark.svg`.
- **Fondo claro (facturas, PDF, papel):** `mark-navy.svg` / `lockup-horizontal-light.svg`.
- **1 tinta / grabado / fax:** `mark-mono.svg`.
- **Avatar redes (IG/X/LinkedIn):** `avatar-gradient-1024.png` (o `avatar-white`).
- **Favicon / app icon:** `favicon.svg`, `favicon-32.png`, `apple-touch-icon-180.png`.

## Favicon en el sitio
```html
<link rel="icon" type="image/svg+xml" href="/favicon.svg">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32.png">
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon-180.png">
```

## Notas de criterio (importante)
- El **navy `#122A4D` es la identidad real** del logo; el degradé es un *tratamiento*, no el logo.
  No uses el degradé como única versión: a tamaños chicos pierde legibilidad y en impresión a 1 tinta no existe.
- A ≤32px el degradé adentro de la boina se ensucia. Para favicon real conviene la versión blanca
  sobre el cuadrado con degradé (ya viene así en `favicon.svg`).
- El wordmark está hecho con **FreeSans Bold** (clon de Helvetica) como placeholder.
  Si tu sitio usa otra tipo en el nav, decime cuál y rehago los lockups con esa fuente outlineada.
