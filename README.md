# README — Secciones Personalizadas para Dawn Theme

Este tema incluye tres secciones personalizadas que extienden las funcionalidades del tema **Dawn** en Shopify.  

## Estructura de archivos

```
/sections/banner-slider.liquid
/assets/section-banner-slider.css

/sections/mosaic-grid.liquid
/assets/section-mosaic-grid.css

/sections/slider-logo.liquid
/assets/section-slider-logo.css
/snippets/slider-logo-item.liquid
```

---

## 1.- Banner Slider
**Archivos:**  
- `sections/banner-slider.liquid`  
- `assets/section-banner-slider.css`

**Descripción:**  
Un slider adaptable para **Desktop/Móvil** con autoplay, controles (anterior, siguiente, dots, play/pause) y soporte táctil.  

**Configuración (desde el editor):**  
- Ancho de la sección: completo o estándar.  
- Activar/desactivar autoplay.  
- Velocidad de transición (3–10s).  
- Bloques: añadir **slides** con imagen Desktop, imagen Móvil, link opcional y texto accesible.  

**Notas:**  
- Detecta viewport para mostrar versión móvil o desktop.  
- CSS incluye *prefers-reduced-motion* y modo oscuro.  

---

## 2.- Mosaico de Contenido
**Archivos:**  
- `sections/mosaic-grid.liquid`  
- `assets/section-mosaic-grid.css`

**Descripción:**  
Un mosaico de **1 bloque grande** + hasta **4 bloques pequeños**. Cada tile puede tener imagen o gradiente, título, descripción, botón, y opcionalmente un ícono decorativo en SVG.  

**Configuración (desde el editor):**  
- Ancho de la sección: completo o estándar.  
- Espaciado superior e inferior.  
- Bloques:  
  - **Mosaico Grande**: título, descripción, botón, imagen o gradiente.  
  - **Mosaico Pequeño**: hasta 4, con esquema de color (oscuro, azul, verde, morado o personalizado).  

**Notas:**  
- CSS trae animaciones suaves y *prefers-reduced-motion*.  

---

## 3.- Carrusel de Logos (Marquee)
**Archivos:**  
- `sections/slider-logo.liquid`  
- `assets/section-slider-logo.css`  
- `snippets/slider-logo-item.liquid`

**Descripción:**  
Un carrusel horizontal continuo de logos, duplicado automáticamente para efecto “marquee infinito”. Incluye encabezado opcional (con degradado o color sólido).  

**Configuración (desde el editor):**  
- Mostrar/ocultar encabezado.  
- Texto, fuente, tamaño, color y radio del encabezado.  
- Fondo sólido o degradado.  
- Ancho y espaciado de cada logo.  
- Velocidad de scroll (8–120s).  
- Pausar al pasar el cursor.  
- Bloques: añadir **logos** (imagen, enlace opcional, alt).  

**Notas:**  
- El snippet `slider-logo-item.liquid` resuelve el texto alternativo evitando errores de Liquid.  

---

## Instalación rápida

1. Copia cada archivo en su carpeta:

```
/sections/banner-slider.liquid
/sections/mosaic-grid.liquid
/sections/slider-logo.liquid
/assets/section-banner-slider.css
/assets/section-mosaic-grid.css
/assets/section-slider-logo.css
/snippets/slider-logo-item.liquid
```

2. En el editor de tema de Shopify → *Añadir sección* → selecciona:  
   - “Banner Slider”  
   - “Mosaico de Contenido”  
   - “Carrusel de Logos”  

3. Configura los bloques y estilos desde el panel visual.
