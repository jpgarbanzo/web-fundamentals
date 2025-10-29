# 📚 Proyecto Final - Portafolio Personal Responsivo

## 🎯 Objetivo

Crear un sitio web de portafolio personal completamente funcional y responsivo que demuestre el dominio de todos los conceptos de HTML y CSS aprendidos en el curso (excepto CSS Grid).

## 📋 Descripción del Proyecto

Desarrollarás un portafolio personal de una página (single-page) con múltiples secciones que incluya información sobre ti, tus habilidades, proyectos y formas de contacto. El sitio debe ser completamente responsivo y utilizar las mejores prácticas de HTML semántico y CSS moderno.

---

## ✅ Requisitos Obligatorios

### 1. Estructura HTML (html-structure.html)

#### DOCTYPE y Estructura Base
- [ ] Declaración `<!DOCTYPE html>` correcta
- [ ] Etiqueta `<html>` con atributo `lang="es"`
- [ ] Sección `<head>` completa con:
  - Meta charset UTF-8
  - Meta viewport para diseño responsivo
  - Título descriptivo de la página
  - Enlace a hoja de estilos CSS externa
  - (Opcional) Favicon
- [ ] Estructura de `<body>` bien organizada

### 2. HTML Semántico (semantic-html.html)

El sitio debe utilizar las siguientes etiquetas semánticas:

- [ ] `<header>` - Cabecera principal con navegación
- [ ] `<nav>` - Menú de navegación con enlaces a secciones
- [ ] `<main>` - Contenido principal del sitio
- [ ] `<section>` - Mínimo 4 secciones diferentes:
  - Sección "Hero" o presentación
  - Sección "Sobre mí"
  - Sección "Habilidades"
  - Sección "Proyectos"
  - Sección "Contacto"
- [ ] `<article>` - Para cada proyecto individual
- [ ] `<aside>` - Información complementaria (opcional)
- [ ] `<footer>` - Pie de página con información de copyright y redes sociales
- [ ] `<figure>` y `<figcaption>` - Para imágenes con descripciones

### 3. Selectores CSS (css-selectors.html)

Debe demostrar el uso de diversos selectores:

- [ ] **Selectores de tipo**: `h1`, `p`, `section`
- [ ] **Selectores de clase**: `.card`, `.button`, `.container`
- [ ] **Selectores de ID**: `#hero`, `#about`, `#contact`
- [ ] **Selectores descendientes**: `nav a`, `.card p`
- [ ] **Selectores de hijo directo**: `nav > ul > li`
- [ ] **Selectores de hermano adyacente**: `h2 + p`
- [ ] **Selectores de atributo**: `a[href^="https"]`, `input[type="email"]`
- [ ] **Pseudo-clases**: `:hover`, `:focus`, `:nth-child()`, `:first-child`, `:last-child`
- [ ] **Pseudo-elementos**: `::before`, `::after`, `::first-line`

### 4. Propiedades CSS (css-properties.html)

Aplicar una variedad de propiedades CSS:

#### Tipografía
- [ ] `font-family` con fallback fonts
- [ ] `font-size`, `font-weight`, `font-style`
- [ ] `line-height` para mejorar legibilidad
- [ ] `text-align`, `text-decoration`, `text-transform`
- [ ] `letter-spacing` o `word-spacing`

#### Colores y Fondos
- [ ] `color` en diferentes formatos (hex, rgb, rgba)
- [ ] `background-color`
- [ ] `background-image` con gradientes
- [ ] `background-size`, `background-position`

#### Modelo de Caja
- [ ] `margin` y `padding` (con diferentes unidades)
- [ ] `border` con estilos variados
- [ ] `border-radius` para esquinas redondeadas
- [ ] `box-shadow` para sombras
- [ ] `width`, `height`, `max-width`, `min-height`

#### Efectos Visuales
- [ ] `opacity` o `rgba` para transparencias
- [ ] `transform` (scale, rotate, translate)
- [ ] `transition` para animaciones suaves
- [ ] Opcional: `animation` con `@keyframes`

### 5. Unidades de Medida (measurements.html)

Utilizar diferentes unidades de medida apropiadamente:

- [ ] **Unidades absolutas**: `px` para bordes y detalles precisos
- [ ] **Unidades relativas**:
  - `em` o `rem` para tipografía
  - `%` para anchos y layouts
  - `vh` y `vw` para secciones de altura completa
- [ ] **Calculaciones**: `calc()` para dimensiones dinámicas
- [ ] Justificar el uso de cada unidad según el contexto

### 6. Flexbox (flexbox.html)

Implementar Flexbox en múltiples secciones:

- [ ] **Navegación horizontal** con Flexbox
  - `display: flex`
  - `justify-content` y `align-items`
  - Espaciado entre elementos

- [ ] **Galería de proyectos** con tarjetas flexibles
  - Contenedor flex con `flex-wrap: wrap`
  - Tarjetas con `flex: 1` o proporciones específicas
  - `gap` para espaciado entre elementos

- [ ] **Sección de habilidades** con iconos/badges
  - Distribución uniforme con `justify-content: space-around`
  - Alineación vertical y horizontal

- [ ] **Footer** con layout flex
  - Múltiples columnas usando flex
  - Alineación de contenido

#### Propiedades Flexbox Requeridas:
- [ ] `display: flex`
- [ ] `flex-direction` (row, column)
- [ ] `justify-content` (diferentes valores)
- [ ] `align-items` (diferentes valores)
- [ ] `flex-wrap`
- [ ] `gap` o `margin` para espaciado
- [ ] `flex` en elementos hijos (flex-grow, flex-shrink, flex-basis)

### 7. Z-Index y Contexto de Apilamiento (z-index.html)

Demostrar comprensión del contexto de apilamiento:

- [ ] **Navegación fija** con z-index alto
  - `position: fixed` o `sticky`
  - `z-index` para mantenerla sobre el contenido

- [ ] **Modal o menú hamburguesa** (para móvil)
  - Overlay con z-index específico
  - Contenido del modal con z-index mayor

- [ ] **Efectos de hover con elevación**
  - Tarjetas que se elevan al hacer hover
  - Uso de `box-shadow` y `transform`
  - Z-index para controlar superposición

- [ ] **Elementos decorativos**
  - Elementos con `::before` o `::after`
  - Posicionamiento y z-index controlado

### 8. Diseño Responsivo (responsive-web.html)

Crear un diseño completamente adaptable:

#### Media Queries
- [ ] **Mobile First**: Estilos base para móviles
- [ ] **Tablet** (min-width: 768px):
  - Ajustar navegación
  - Cambiar layout de 1 columna a 2 columnas
  - Aumentar tamaños de fuente

- [ ] **Desktop** (min-width: 1024px):
  - Layout de 3 columnas para galería
  - Navegación expandida
  - Espaciado mejorado

- [ ] **Desktop grande** (min-width: 1440px):
  - Max-width para contenedor principal
  - Ajustes de tipografía

#### Técnicas Responsivas
- [ ] Imágenes responsivas con `max-width: 100%`
- [ ] Unidades relativas (rem, em, %) en lugar de px fijos
- [ ] Flexbox con `flex-wrap` para adaptabilidad
- [ ] `clamp()` para tamaños de fuente fluidos (opcional)
- [ ] Navegación móvil (menú hamburguesa)

#### Breakpoints Mínimos Requeridos:
```css
/* Mobile: 320px - 767px (estilos por defecto) */

/* Tablet */
@media (min-width: 768px) {
  /* Estilos para tablet */
}

/* Desktop */
@media (min-width: 1024px) {
  /* Estilos para desktop */
}

/* Desktop Grande */
@media (min-width: 1440px) {
  /* Estilos para pantallas grandes */
}
```

---

## 🎨 Contenido Sugerido por Sección

### 1. Header/Navegación
- Logo o nombre personal
- Menú de navegación con enlaces a todas las secciones
- Efecto sticky o fixed para que permanezca visible

### 2. Sección Hero/Presentación
- Título con tu nombre
- Subtítulo con tu profesión/ocupación
- Breve frase descriptiva
- Botón CTA (Call to Action) que lleve a la sección de contacto
- Imagen de perfil o ilustración
- Fondo atractivo (gradiente, imagen, o color sólido)

### 3. Sección "Sobre Mí"
- Párrafos describiendo tu experiencia, educación, intereses
- Foto personal (opcional)
- Información relevante presentada de forma atractiva

### 4. Sección "Habilidades"
- Lista de tecnologías/habilidades técnicas
- Representadas con iconos, badges, o barras
- Uso de Flexbox para distribución
- Mínimo 6-8 habilidades

### 5. Sección "Proyectos"
- Mínimo 3 proyectos
- Cada proyecto debe tener:
  - Imagen representativa
  - Título
  - Descripción breve
  - Tecnologías utilizadas
  - Enlaces (GitHub, demo, etc.)
- Tarjetas con efecto hover
- Layout responsivo con Flexbox

### 6. Sección "Contacto"
- Formulario de contacto con:
  - Campo nombre
  - Campo email
  - Campo mensaje/textarea
  - Botón submit
- Validación HTML5 (required, type="email")
- Enlaces a redes sociales
- Información de contacto alternativa

### 7. Footer
- Copyright con año actual
- Enlaces a redes sociales
- Enlaces adicionales de navegación
- Información de contacto resumida

---

## 🎯 Criterios de Evaluación

### HTML Semántico (20 puntos)
- Uso correcto de etiquetas semánticas (10 pts)
- Estructura HTML válida y bien organizada (5 pts)
- Accesibilidad básica (atributos alt, labels) (5 pts)

### CSS Selectores y Propiedades (20 puntos)
- Variedad de selectores utilizados apropiadamente (10 pts)
- Aplicación correcta de propiedades CSS (5 pts)
- Uso apropiado de unidades de medida (5 pts)

### Flexbox (15 puntos)
- Implementación correcta en navegación (5 pts)
- Galería de proyectos con Flexbox (5 pts)
- Uso de propiedades flex variadas (5 pts)

### Z-Index y Posicionamiento (10 puntos)
- Navegación fija/sticky funcional (5 pts)
- Correcta gestión del contexto de apilamiento (5 pts)

### Diseño Responsivo (20 puntos)
- Mobile-first approach (5 pts)
- Media queries correctamente implementadas (8 pts)
- Adaptación adecuada en diferentes dispositivos (7 pts)

### Diseño Visual y Creatividad (10 puntos)
- Paleta de colores coherente (3 pts)
- Tipografía legible y atractiva (3 pts)
- Creatividad en el diseño (4 pts)

### Calidad del Código (5 puntos)
- Código limpio y organizado (3 pts)
- Comentarios donde sea necesario (2 pts)

---

## 📦 Entregables

### Estructura de Archivos Requerida:
```
portafolio/
├── index.html
├── styles.css
├── images/
│   ├── profile.jpg
│   ├── project1.jpg
│   ├── project2.jpg
│   └── project3.jpg
└── README.md (opcional)
```

### Documentos a Entregar:
1. **Código fuente completo** (HTML + CSS)
2. **Imágenes utilizadas** en carpeta organizada
3. **Archivo README.md** (opcional) explicando:
   - Descripción del proyecto
   - Tecnologías utilizadas
   - Conceptos aplicados
   - Instrucciones para visualizar

---

## 🚀 Pasos Recomendados para Desarrollar el Proyecto

### Fase 1: Planificación (Día 1)
1. Diseñar wireframe básico en papel o herramienta digital
2. Definir paleta de colores
3. Seleccionar tipografías
4. Recopilar contenido (textos, imágenes)

### Fase 2: Estructura HTML (Día 2)
1. Crear estructura HTML completa
2. Agregar contenido semántico
3. Validar HTML

### Fase 3: Estilos Base (Día 3)
1. Crear CSS reset/normalize
2. Definir variables CSS (colores, fuentes)
3. Estilos de tipografía base
4. Estilos mobile-first

### Fase 4: Layouts con Flexbox (Día 4)
1. Implementar navegación
2. Crear sección hero
3. Diseñar galería de proyectos
4. Construir footer

### Fase 5: Responsividad (Día 5)
1. Agregar media queries para tablet
2. Agregar media queries para desktop
3. Probar en diferentes dispositivos
4. Ajustar breakpoints según necesidad

### Fase 6: Detalles Finales (Día 6)
1. Agregar efectos hover y transiciones
2. Implementar z-index en navegación
3. Refinar espaciado y alineación
4. Optimizar imágenes

### Fase 7: Pruebas y Ajustes (Día 7)
1. Validar HTML y CSS
2. Probar en diferentes navegadores
3. Verificar accesibilidad básica
4. Hacer ajustes finales

---

## 💡 Consejos y Mejores Prácticas

### HTML
- Usa nombres descriptivos para clases e IDs
- Mantén la jerarquía de encabezados (h1, h2, h3...)
- Agrega atributos `alt` descriptivos a todas las imágenes
- Usa etiquetas semánticas en lugar de `<div>` cuando sea apropiado

### CSS
- Organiza tu CSS por secciones (comentarios claros)
- Usa metodología consistente para nombres de clases (BEM, o similar)
- Evita selectores demasiado específicos
- Prefiere clases sobre IDs para estilos
- Agrupa propiedades relacionadas

### Flexbox
- Recuerda que `justify-content` controla el eje principal
- `align-items` controla el eje transversal
- Usa `gap` en lugar de margins cuando sea posible
- `flex-wrap: wrap` es tu aliado para diseños responsivos

### Responsividad
- Prueba constantemente en diferentes tamaños
- Usa herramientas de desarrollo del navegador
- Considera puntos de quiebre basados en tu contenido, no solo en dispositivos comunes
- Las imágenes deben ser fluidas (`max-width: 100%`)

### Rendimiento
- Optimiza imágenes (tamaño y formato)
- Minimiza el uso de efectos costosos
- Usa transiciones en propiedades específicas, no `all`

---

## 🔍 Recursos Adicionales

### Validadores
- HTML: https://validator.w3.org/
- CSS: https://jigsaw.w3.org/css-validator/

### Herramientas de Prueba Responsiva
- Chrome DevTools (F12 > Toggle Device Toolbar)
- Firefox Responsive Design Mode
- https://responsivedesignchecker.com/

### Inspiración de Diseño
- https://dribbble.com/tags/portfolio
- https://www.awwwards.com/websites/portfolio/
- https://codepen.io/search/pens?q=portfolio

### Colores y Tipografía
- Google Fonts: https://fonts.google.com/
- Coolors (paletas): https://coolors.co/
- Adobe Color: https://color.adobe.com/

### Imágenes Gratuitas
- Unsplash: https://unsplash.com/
- Pexels: https://www.pexels.com/
- Pixabay: https://pixabay.com/

---

## ⚠️ Restricciones Importantes

### NO Permitido:
- ❌ Uso de CSS Grid (se cubrirá en módulo futuro)
- ❌ Frameworks CSS (Bootstrap, Tailwind, etc.)
- ❌ JavaScript (a menos que sea para funcionalidad básica opcional)
- ❌ Copiar código de templates existentes

### SÍ Permitido:
- ✅ Consultar documentación (MDN, W3Schools)
- ✅ Usar referencias visuales para inspiración
- ✅ Iconos de bibliotecas externas (Font Awesome, opcional)
- ✅ Google Fonts para tipografía
- ✅ Creatividad y diseño personalizado

---

## 📅 Fecha de Entrega

**[Definir según el calendario del curso]**

---

## ❓ Preguntas Frecuentes

**P: ¿Puedo usar más de una página HTML?**
R: El proyecto debe ser de una sola página (single-page), pero puedes tener páginas adicionales para proyectos individuales si lo deseas (opcional).

**P: ¿Cuánto código CSS es suficiente?**
R: No hay un mínimo, pero debes demostrar dominio de todos los conceptos listados. Un portafolio bien diseñado típicamente requiere 300-600 líneas de CSS.

**P: ¿Puedo usar preprocesadores como SASS?**
R: Se recomienda usar CSS puro para demostrar conocimientos fundamentales, pero si conoces SASS puedes usarlo.

**P: ¿Qué hago si no tengo proyectos reales para mostrar?**
R: Puedes crear proyectos ficticios o mostrar ejercicios del curso como proyectos de práctica.

**P: ¿Es obligatorio hacer un menú hamburguesa para móvil?**
R: Se recomienda encarecidamente para una buena experiencia móvil, pero puedes usar navegación colapsada o simplificada.

**P: ¿Puedo usar JavaScript para el menú hamburguesa?**
R: Sí, es aceptable usar JavaScript básico para funcionalidad interactiva como un menú hamburguesa o modal.

---

## 🎓 Criterios de Excelencia

Para obtener la máxima calificación, tu proyecto debe:

1. ✨ **Código impecable**: HTML válido, CSS organizado y comentado
2. 🎨 **Diseño profesional**: Visualmente atractivo y coherente
3. 📱 **Perfectamente responsivo**: Funciona perfectamente en todos los dispositivos
4. ♿ **Accesible**: Considera usuarios con diferentes capacidades
5. ⚡ **Optimizado**: Imágenes optimizadas, código eficiente
6. 🚀 **Creativo**: Muestra personalidad y originalidad
7. 📚 **Completo**: Incluye todas las secciones y requisitos
8. 🎯 **Funcional**: Todos los enlaces y formularios funcionan

---

## 🏆 Bonus (Puntos Extras)

Características opcionales que pueden darte puntos adicionales:

- [ ] **Modo oscuro/claro** con botón toggle (requiere JavaScript)
- [ ] **Animaciones avanzadas** con @keyframes
- [ ] **Sección de testimonios** con diseño creativo
- [ ] **Parallax scrolling** sutil
- [ ] **Iconos personalizados** SVG en línea
- [ ] **Carga progresiva** de contenido con efectos
- [ ] **Formulario de contacto funcional** (requiere backend o servicio)
- [ ] **Optimización SEO** (meta tags, estructura semántica avanzada)
- [ ] **Rendimiento optimizado** (imágenes WebP, lazy loading)
- [ ] **Variables CSS (Custom Properties)** para temas

---

## 📞 Soporte

Si tienes dudas durante el desarrollo:

1. Revisa las lecciones correspondientes del curso
2. Consulta la documentación de MDN
3. Participa en foros de discusión del curso
4. Contacta al instructor durante horario de oficina

---

## ✅ Checklist Final Antes de Entregar

- [ ] HTML validado sin errores
- [ ] CSS validado sin errores
- [ ] Probado en Chrome, Firefox, y Safari
- [ ] Responsivo en móvil, tablet y desktop
- [ ] Todas las imágenes tienen atributo alt
- [ ] Navegación funciona correctamente
- [ ] Enlaces se abren apropiadamente (externos en nueva pestaña)
- [ ] Formulario tiene validación básica
- [ ] Código comentado donde es necesario
- [ ] Sin errores en la consola del navegador
- [ ] Archivos organizados correctamente
- [ ] README incluido (si aplica)

---

## 🎉 ¡Mucho Éxito!

Este proyecto es tu oportunidad para demostrar todo lo que has aprendido y crear algo de lo que puedas estar orgulloso. Tómate el tiempo necesario, presta atención a los detalles, y no tengas miedo de ser creativo.

**Recuerda**: Este portafolio puede ser la base de tu presencia profesional en línea. ¡Hazlo brillar! ✨

---

**© 2024 - Proyecto Final del Curso de Fundamentos Web**
