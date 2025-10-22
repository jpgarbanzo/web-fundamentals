# Web Fundamentals Lesson Guidelines

This document provides instructions for creating new interactive lesson files that are consistent with existing lessons (flexbox.html, grid.html, z-index.html, semantic-html.html).

## File Structure

Each lesson file should be a self-contained HTML file with:
- Embedded CSS in `<style>` tags
- Embedded JavaScript for slideshow functionality
- All content in Spanish (es)

## Naming Convention

- Use lowercase with hyphens: `lesson-topic.html`
- Examples: `flexbox.html`, `grid.html`, `z-index.html`, `semantic-html.html`

## Document Structure

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Topic] - Presentación Interactiva</title>
    <style>
        /* All styles here */
    </style>
</head>
<body>
    <div class="slideshow-container">
        <!-- Slides here -->

        <!-- Controls (always last) -->
        <div class="controls">
            <button id="prevBtn" onclick="changeSlide(-1)">← Anterior</button>
            <span class="slide-counter"><span id="currentSlide">1</span> / <span id="totalSlides">10</span></span>
            <button id="nextBtn" onclick="changeSlide(1)">Siguiente →</button>
        </div>
    </div>

    <script>
        /* Slideshow logic here */
    </script>
</body>
</html>
```

## Slide Count

- Aim for **10-12 slides** per lesson
- Minimum: 10 slides
- Maximum: 15 slides (only if topic is very complex)

## Slide Structure

### Slide 1: Title Slide
```html
<div class="slide active">
    <h1>🎯 Introducción a [Topic]</h1>
    <p style="font-size: 1.5em; margin-top: 40px;">Descripción breve atractiva</p>
    <p style="margin-top: 60px;">Párrafo de introducción explicando qué es...</p>
    <p>Párrafo adicional con contexto o importancia...</p>
</div>
```

### Slide 2: ¿Qué es? / Conceptos Clave
```html
<div class="slide">
    <h2>¿Qué es [Topic]?</h2>
    <p>Definición clara...</p>

    <div class="code">
        /* Código de ejemplo básico */
    </div>

    <p><strong>Conceptos clave:</strong></p>
    <ul>
        <li><span class="property">Concepto 1:</span> Explicación</li>
        <li><span class="property">Concepto 2:</span> Explicación</li>
    </ul>
</div>
```

### Slides 3-8: Contenido Principal
- Cada slide enfocada en un concepto específico
- Incluir código de ejemplo
- Incluir demostración visual cuando sea posible
- Usar `<div class="demo-container">` para demostraciones

### Slide 9: Casos de Uso
```html
<div class="slide">
    <h2>Casos de Uso Comunes</h2>
    <ul>
        <li><strong>Caso 1:</strong> Descripción y propiedades relevantes</li>
        <li><strong>Caso 2:</strong> Descripción y propiedades relevantes</li>
        <!-- ... -->
    </ul>
    <p style="margin-top: 40px;">Comentario final sobre cuándo usar...</p>
</div>
```

### Última Slide: Conclusión
```html
<div class="slide">
    <h2>🎉 ¡Domina [Topic]!</h2>

    <p style="font-size: 1.3em; margin-top: 40px;"><strong>Puntos clave para recordar:</strong></p>

    <ul style="margin-top: 30px;">
        <li>Punto clave 1</li>
        <li>Punto clave 2</li>
        <!-- 5-7 puntos clave -->
    </ul>

    <p style="margin-top: 60px; font-size: 1.2em; color: #667eea; text-align: center;">
        <strong>¡Mensaje motivacional final!</strong>
    </p>
</div>
```

## CSS Styling Standards

### Core Styles (Required)

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    padding: 20px;
}

.slideshow-container {
    max-width: 900px;
    width: 100%;
    background: white;
    border-radius: 20px;
    box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
    overflow: hidden;
}

.slide {
    display: none;
    padding: 60px;
    min-height: 600px;
}

.slide.active {
    display: block;
    animation: fadeIn 0.5s;
}

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}
```

### Typography Standards

```css
h1 {
    color: #667eea;
    font-size: 2.5em;
    margin-bottom: 20px;
}

h2 {
    color: #764ba2;
    font-size: 2em;
    margin-bottom: 30px;
}

p {
    font-size: 1.2em;
    line-height: 1.8;
    color: #333;
    margin-bottom: 20px;
}

ul {
    margin-left: 30px;
    margin-bottom: 20px;
}

li {
    font-size: 1.1em;
    line-height: 1.8;
    color: #333;
    margin-bottom: 10px;
}
```

### Special Elements

```css
/* Code blocks */
.code {
    background: #f5f5f5;
    border-left: 4px solid #667eea;
    padding: 15px;
    margin: 20px 0;
    font-family: 'Courier New', monospace;
    border-radius: 5px;
}

/* Demo containers */
.demo-container {
    border: 2px solid #667eea;
    padding: 20px;
    margin: 20px 0;
    border-radius: 10px;
    background: #f9f9f9;
}

/* Highlighted text */
.highlight {
    background: #fff3cd;
    padding: 2px 6px;
    border-radius: 3px;
}

/* Property names */
.property {
    color: #764ba2;
    font-weight: bold;
}
```

### Controls (Required)

```css
.controls {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px 60px;
    background: #f5f5f5;
}

button {
    background: #667eea;
    color: white;
    border: none;
    padding: 15px 30px;
    font-size: 1.1em;
    border-radius: 10px;
    cursor: pointer;
    transition: all 0.3s;
}

button:hover {
    background: #764ba2;
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
}

button:disabled {
    background: #ccc;
    cursor: not-allowed;
    transform: none;
}

.slide-counter {
    font-size: 1.2em;
    color: #667eea;
    font-weight: bold;
}
```

## Color Palette

### Primary Colors
- **Purple gradient**: `#667eea` to `#764ba2`
- **Main purple**: `#667eea`
- **Dark purple**: `#764ba2`

### Demo Colors (use for interactive examples)
- Red: `#ef4444`
- Blue: `#3b82f6`
- Green: `#10b981`
- Orange: `#f59e0b`
- Purple: `#8b5cf6`

### Background Colors
- Light purple: `#e0e7ff`
- Light gray: `#f9f9f9`
- Code background: `#f5f5f5`

## JavaScript (Required - Copy Exactly)

```javascript
let currentSlide = 0;
const slides = document.querySelectorAll('.slide');
const totalSlides = slides.length;

document.getElementById('totalSlides').textContent = totalSlides;

function showSlide(n) {
    slides[currentSlide].classList.remove('active');

    if (n >= totalSlides) {
        currentSlide = totalSlides - 1;
    } else if (n < 0) {
        currentSlide = 0;
    } else {
        currentSlide = n;
    }

    slides[currentSlide].classList.add('active');
    document.getElementById('currentSlide').textContent = currentSlide + 1;

    // Actualizar estado de botones
    document.getElementById('prevBtn').disabled = currentSlide === 0;
    document.getElementById('nextBtn').disabled = currentSlide === totalSlides - 1;
}

function changeSlide(direction) {
    showSlide(currentSlide + direction);
}

// Navegación con teclado
document.addEventListener('keydown', (e) => {
    if (e.key === 'ArrowLeft') changeSlide(-1);
    if (e.key === 'ArrowRight') changeSlide(1);
});

// Inicializar
showSlide(0);
```

## Interactive Demos

### Basic Demo Structure
```html
<div class="demo-container">
    <p><strong>Título de la demo:</strong></p>
    <div class="demo-specific-class">
        <!-- Demo content -->
    </div>
</div>
```

### Demo Styling Guidelines
- Background: `#e0e7ff` (light purple)
- Items inside demo: Use color palette colors
- Padding: `15px` for demo area, `20px` for container
- Border radius: `8px` for demo area

## Code Examples

### Inline Code
Use `<span class="highlight">` for inline code references:
```html
<p>Use la propiedad <span class="highlight">display: flex</span> para activar flexbox.</p>
```

### Code Blocks
```html
<div class="code">
    .selector {<br>
    &nbsp;&nbsp;property: value;<br>
    }
</div>
```

**Important**: Use `<br>` for line breaks and `&nbsp;` for indentation (2 spaces = `&nbsp;&nbsp;`)

## Language and Tone

### Language
- **All content in Spanish**
- Use formal "tú" form, not "usted"
- Technical terms can remain in English when commonly used (e.g., "flexbox", "grid")

### Tone
- Educational and encouraging
- Clear and concise explanations
- Use emojis sparingly (mainly in title and conclusion slides)
- Professional but friendly

### Common Phrases
- "¿Qué es...?" (What is...?)
- "Conceptos clave" (Key concepts)
- "Casos de Uso Comunes" (Common use cases)
- "Puntos clave para recordar" (Key points to remember)
- "¡Domina [Topic]!" (Master [Topic]!)

## Special Elements

### Warning Boxes
```html
<div class="warning">
    <strong>⚠️ Importante:</strong> Mensaje importante aquí...
</div>
```

CSS:
```css
.warning {
    background: #fef3c7;
    border-left: 4px solid #f59e0b;
    padding: 15px;
    margin: 20px 0;
    border-radius: 5px;
}
```

### Comparison (Good vs Bad)
```html
<div class="comparison">
    <div class="bad-example">
        <strong>❌ No recomendado:</strong>
        <!-- Content -->
    </div>
    <div class="good-example">
        <strong>✅ Recomendado:</strong>
        <!-- Content -->
    </div>
</div>
```

CSS:
```css
.comparison {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 15px;
    margin: 20px 0;
}

.bad-example {
    background: #fee;
    border-left: 4px solid #ef4444;
    padding: 15px;
    border-radius: 5px;
}

.good-example {
    background: #efe;
    border-left: 4px solid #10b981;
    padding: 15px;
    border-radius: 5px;
}
```

## Content Guidelines

### Slide 1 - Title
- Use emoji (🎯 recommended)
- Format: "Introducción a [Topic]"
- Include 2-3 paragraphs of introduction
- Explain WHAT it is and WHY it matters

### Slides 2-3 - Fundamentals
- Define the topic clearly
- Include basic code example
- List key concepts with bullet points
- Use `.property` class for technical terms

### Slides 4-8 - Core Concepts
- One main concept per slide
- Always include code example
- Include visual demo when possible
- Keep explanations concise but complete

### Slide 9 - Use Cases
- 5-7 practical use cases
- Format: **Use Case:** Description with relevant properties
- End with summary statement about when to use

### Final Slide - Conclusion
- Title: "🎉 ¡Domina [Topic]!"
- "Puntos clave para recordar:" heading
- 5-7 key bullet points (summary of most important concepts)
- Motivational closing message centered at bottom

## Accessibility

- Use semantic HTML structure
- Maintain heading hierarchy (h1 → h2, no skipping)
- Ensure sufficient color contrast
- Button states (disabled) are visually clear
- Keyboard navigation supported (arrow keys)

## Testing Checklist

Before considering a lesson complete, verify:

- [ ] File opens without errors in browser
- [ ] All slides display correctly
- [ ] Navigation buttons work (Previous/Next)
- [ ] Keyboard navigation works (Left/Right arrows)
- [ ] First slide shows "Previous" button as disabled
- [ ] Last slide shows "Next" button as disabled
- [ ] Slide counter updates correctly
- [ ] All code examples are properly formatted
- [ ] All demos display as intended
- [ ] Responsive on mobile (check at 375px width)
- [ ] All text is in Spanish
- [ ] No console errors
- [ ] Colors match the established palette

## Example Topics for Future Lessons

Potential topics that would fit this format:
- `position.html` - CSS positioning (static, relative, absolute, fixed, sticky)
- `responsive-design.html` - Media queries and responsive techniques
- `css-variables.html` - CSS custom properties
- `transitions.html` - CSS transitions and animations
- `forms.html` - HTML forms and validation
- `css-selectors.html` - Advanced CSS selectors
- `box-model.html` - CSS box model
- `pseudo-elements.html` - ::before, ::after, etc.
- `css-functions.html` - calc(), var(), clamp(), etc.
- `accessibility.html` - Web accessibility (ARIA, best practices)

## Quick Start Template

To create a new lesson quickly:

1. Copy `flexbox.html` as your starting point
2. Update the `<title>` tag
3. Replace slide 1 title and content
4. Update total slide count in controls
5. Replace slides 2-9 with your content
6. Update final slide with topic-specific points
7. Add topic-specific demo styles
8. Test all functionality

## Questions?

When in doubt:
- Refer to existing lesson files for examples
- Keep it simple and clear
- Prioritize educational value over complexity
- Maintain visual and structural consistency
