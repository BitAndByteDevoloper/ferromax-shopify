# README — Secciones Personalizadas para Dawn Theme

Este repositorio incluye **seis secciones personalizadas** que amplían y enriquecen el tema **Dawn** de Shopify. Cada sección ha sido diseñada para mejorar la experiencia visual, de navegación y de comunicación, ofreciendo mayor flexibilidad a nivel de diseño y contenido.  

## 📂 Estructura de archivos

```
/sections/banner-slider.liquid
/assets/section-banner-slider.css

/sections/mosaic-grid.liquid
/assets/section-mosaic-grid.css

/sections/slider-logo.liquid
/assets/section-slider-logo.css
/snippets/slider-logo-item.liquid

/sections/blank-space.liquid

/sections/dynamic-phrases.liquid
/assets/section-dynamic-phrases.css

/sections/icons-benefits.liquid
/assets/section-icons-benefits.css
```

---

## 1.- Banner Slider
**Archivos:**  
- `sections/banner-slider.liquid`  
- `assets/section-banner-slider.css`

**Descripción:**  
El **Banner Slider** es una sección de carrusel pensada para mostrar imágenes destacadas en la tienda (ej. promociones, campañas o branding). Es **totalmente responsivo**, adaptándose a escritorio y dispositivos móviles. Incluye **autoplay configurable**, controles de navegación (anterior, siguiente, indicadores de slide y pausa/play), así como soporte táctil para una experiencia fluida en móvil.  

Este slider detecta el viewport y carga la versión correcta (Desktop/Móvil). Su CSS incorpora soporte para *prefers-reduced-motion* y modo oscuro, optimizando accesibilidad y usabilidad.  

**Configuración:**  
- Ancho de la sección (completo o estándar).  
- Autoplay: activar/desactivar + velocidad de transición (3–10s).  
- Bloques de slide con:  
  - Imagen Desktop (recomendado 1400x400).  
  - Imagen Móvil (recomendado 800x800).  
  - Enlace opcional y abrir en nueva pestaña.  
  - Texto alternativo para accesibilidad.  

---

## 2.- Mosaico de Contenido
**Archivos:**  
- `sections/mosaic-grid.liquid`  
- `assets/section-mosaic-grid.css`

**Descripción:**  
El **Mosaico de Contenido** permite mostrar información en un **layout flexible** compuesto por un mosaico grande y hasta cuatro mosaicos pequeños. Es ideal para destacar productos, categorías, beneficios o servicios.  

Cada mosaico admite **imagen o gradiente de colores**, y se pueden añadir etiquetas, títulos, descripciones, botones personalizables e íconos SVG decorativos. El CSS ofrece esquemas de color predeterminados (oscuro, azul, verde, morado, personalizado), animaciones suaves y compatibilidad con *prefers-reduced-motion*.  

**Configuración:**  
- Ancho: completo o estándar.  
- Espaciado superior e inferior.  
- Bloques:  
  - **Mosaico Grande**: título, descripción, botón, fondo (imagen/gradiente) e ícono decorativo.  
  - **Mosaicos Pequeños**: hasta 4, con esquema de color configurable.  

---

## 3.- Carrusel de Logos (Marquee)
**Archivos:**  
- `sections/slider-logo.liquid`  
- `assets/section-slider-logo.css`  
- `snippets/slider-logo-item.liquid`

**Descripción:**  
El **Carrusel de Logos** es ideal para mostrar logotipos de marcas, aliados o proveedores. Utiliza un efecto *marquee infinito*, duplicando los logos para mantener un scroll continuo y dinámico.  

Incluye un **encabezado opcional** totalmente configurable (texto, tipografía, color sólido o degradado, tamaño, radio de borde). Es accesible y responsivo, permitiendo pausar el scroll al pasar el cursor.  

**Configuración:**  
- Encabezado: mostrar/ocultar + estilo (texto, tipografía, color, tamaño, degradado o sólido).  
- Logos: ancho, espaciado, velocidad de scroll (8–120s).  
- Bloques de logo: imagen, enlace opcional, alt.  

**Notas:**  
El snippet `slider-logo-item.liquid` asegura que el atributo alt se procese sin errores de Liquid.  

---

## 4.- Espacio en Blanco
**Archivo:**  
- `sections/blank-space.liquid`

**Descripción:**  
La sección de **Espacio en Blanco** es una herramienta utilitaria para agregar **espaciado vertical** entre secciones de la página. Es especialmente útil para ajustar el ritmo visual del layout sin necesidad de modificar el código del tema.  

Incluye un modo “debug” que permite visualizar el área vacía con un fondo semitransparente y un borde punteado de color configurable, lo que facilita ajustar la maquetación durante el desarrollo.  

**Configuración:**  
- Bloques de tipo “Space”.  
- Altura en píxeles (10–500).  
- Mostrar u ocultar color de depuración.  
- Seleccionar color de depuración.  

---

## 5.- Frases Dinámicas
**Archivos:**  
- `sections/dynamic-phrases.liquid`  
- `assets/section-dynamic-phrases.css`

**Descripción:**  
La sección de **Frases Dinámicas** está pensada para mostrar mensajes que cambian con el tiempo o según reglas definidas. Permite añadir múltiples frases que se muestran de manera **rotativa, aleatoria, secuencial o basadas en intervalos de tiempo** (minutos, horas, días, meses).  

Se pueden enfatizar palabras con una clase CSS de acento, incluir íconos (imagen o SVG), y configurar fuente, tamaño, color, espaciado, padding y alineación.  

**Configuración:**  
- Modos de rotación: secuencial, aleatorio, por sesión, por usuario, por tiempo.  
- Intervalo configurable en minutos o segundos.  
- Persistencia de frase aleatoria (por usuario o sesión).  
- Opción de usar el ID del cliente para personalizar.  
- Bloques de frases: texto, link opcional, palabras a enfatizar.  

---

## 6.- Iconos / Beneficios
**Archivos:**  
- `sections/icons-benefits.liquid`  
- `assets/section-icons-benefits.css`

**Descripción:**  
La sección de **Iconos/Beneficios** permite mostrar un conjunto de características o ventajas en un **grid responsivo de iconos con títulos y subtítulos**. Es ideal para comunicar valores agregados, servicios destacados o beneficios de productos.  

Cada ítem puede contener un ícono SVG, un título, un subtítulo y un enlace opcional. El CSS adapta el número de columnas según el dispositivo (4 en desktop, 3 en tablet, 2 en móvil) y permite personalizar colores, tamaños de íconos y tipografía.  

**Configuración:**  
- Grid configurable en columnas y espaciado.  
- Estilos de ícono: SVG escalable o placeholder.  
- Contenido de cada bloque: ícono, título, subtítulo y enlace.  
- Ajustes de alineación, padding y colores de fondo/texto.  

---

## 🚀 Instalación rápida

1. Copia cada archivo en su carpeta correspondiente:

```
/sections/banner-slider.liquid
/sections/mosaic-grid.liquid
/sections/slider-logo.liquid
/sections/blank-space.liquid
/sections/dynamic-phrases.liquid
/sections/icons-benefits.liquid

/assets/section-banner-slider.css
/assets/section-mosaic-grid.css
/assets/section-slider-logo.css
/assets/section-dynamic-phrases.css
/assets/section-icons-benefits.css

/snippets/slider-logo-item.liquid
```

2. En el editor de tema de Shopify → *Añadir sección*, selecciona:  
   - “Banner Slider”  
   - “Mosaico de Contenido”  
   - “Carrusel de Logos”  
   - “Espacio en Blanco”  
   - “Frases Dinamicas con Icono”  
   - “Iconos / Beneficios”  

3. Configura los bloques y estilos desde el panel visual según las necesidades de tu tienda.  
