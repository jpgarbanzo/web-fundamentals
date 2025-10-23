# Web Fundamentals - Interactive Lessons

Interactive slideshow presentations for learning web development fundamentals. All lessons are in Spanish and feature live code examples and visual demonstrations.

## Available Lessons

### CSS Fundamentals

- **[css-properties.html](css-properties.html)** - Common CSS Properties

  - Essential CSS properties every developer should know
  - Color and background properties
  - Typography: font-family, font-size, font-weight, line-height
  - Box model: margin, padding, border, width, height
  - Display, position, and layout properties
  - Visual effects: opacity, transform, box-shadow
  - Shorthand properties for cleaner code
  - 12 slides with live examples and demos

- **[css-selectors.html](css-selectors.html)** - CSS Selectors
  - Complete guide to all CSS selector types
  - Basic selectors: element, class, ID
  - Attribute selectors with patterns
  - Combinators: descendant, child, adjacent, sibling
  - Pseudo-classes: :hover, :focus, :nth-child, :not
  - Pseudo-elements: ::before, ::after, ::first-letter
  - Selector specificity and best practices
  - Modern selectors: :is(), :where(), :has()
  - 12 slides with selector examples and specificity table

### CSS Layout & Positioning

- **[flexbox.html](flexbox.html)** - CSS Flexbox

  - Introduction to flexible box layout
  - Flex container and items concepts
  - Properties: `justify-content`, `align-items`, `flex-direction`, `flex-wrap`
  - Flex item properties: `flex-grow`, `flex-shrink`, `flex-basis`
  - Common use cases and patterns
  - 10 slides with interactive demos

- **[grid.html](grid.html)** - CSS Grid

  - Two-dimensional grid layout system
  - Grid template columns and rows
  - Gap spacing and grid areas
  - Grid template areas for semantic layouts
  - Auto-fit and auto-fill for responsive designs
  - 10 slides with visual layout examples

- **[z-index.html](z-index.html)** - Z-Index & Stacking Context
  - Understanding the z-axis and stacking order
  - How z-index works with positioned elements
  - Stacking contexts and their limitations
  - Common z-index values and organization
  - Use cases: modals, overlays, tooltips
  - 10 slides with overlapping element demos

### Responsive Design

- **[responsive-web.html](responsive-web.html)** - Responsive Web Design
  - Mobile-first design approach
  - Viewport meta tag configuration
  - Media queries and breakpoints
  - Flexible units: %, rem, vw/vh
  - Responsive images and layouts
  - Modern CSS techniques (clamp, auto-fit, container queries)
  - 12 slides with device and layout demonstrations

### Development Tools

- **[git-fundamentals.html](git-fundamentals.html)** - Git Fundamentals
  - Introduction to version control with Git
  - Cloning repositories with `git clone`
  - Basic workflow: add, commit, push, pull
  - Creating and managing branches
  - Merging branches and collaboration
  - Essential Git commands and best practices
  - 12 slides with visual diagrams and terminal examples

### HTML Structure

- **[html-structure.html](html-structure.html)** - HTML Document Structure

  - Anatomy of an HTML document: `<html>`, `<head>`, `<body>`
  - Essential meta tags: charset, viewport, SEO tags
  - Importing CSS: external, internal, and inline styles
  - JavaScript placement: async, defer, and best practices
  - File paths and routes: relative vs absolute
  - Project organization and resource constraints
  - 12 slides with code examples and folder structures

- **[semantic-html.html](semantic-html.html)** - Semantic HTML Tags
  - Importance of semantic HTML for accessibility and SEO
  - Structural tags: `<header>`, `<nav>`, `<main>`, `<aside>`, `<footer>`
  - Content tags: `<article>`, `<section>`, `<figure>`
  - Text semantics: `<strong>`, `<em>`, `<mark>`, `<time>`
  - Form semantics and best practices
  - 12 slides with layout examples and comparisons

## Features

Each lesson includes:

- ✅ **Interactive slideshow** with keyboard navigation (arrow keys)
- ✅ **Live code examples** with syntax highlighting
- ✅ **Visual demonstrations** of concepts
- ✅ **Clear explanations** in Spanish
- ✅ **Consistent design** with purple gradient theme
- ✅ **Responsive layout** for mobile and desktop
- ✅ **Self-contained** - no external dependencies

## How to Use

1. Open any `.html` file in a web browser
2. Navigate using:
   - **Next/Previous buttons** at the bottom
   - **Arrow keys** (← →) on keyboard
3. Review code examples and interactive demos on each slide

## Creating New Lessons

To maintain consistency when adding new lessons:

1. Review the guidelines in `.claude/lesson-guidelines.md`
2. Use `.claude/lesson-template.html` as a starting point
3. Follow the established structure and styling
4. Test with the checklist in the guidelines

Or use the Claude Code slash command:

```
/new-lesson
```

## Project Structure

```
web-fundamentals/
├── css-properties.html    # Common CSS Properties lesson
├── css-selectors.html     # CSS Selectors lesson
├── flexbox.html           # CSS Flexbox lesson
├── grid.html              # CSS Grid lesson
├── z-index.html           # Z-Index lesson
├── responsive-web.html    # Responsive Web Design lesson
├── git-fundamentals.html  # Git version control lesson
├── html-structure.html    # HTML Document Structure lesson
├── semantic-html.html     # Semantic HTML lesson
├── README.md              # This file
└── .claude/
    ├── README.md          # Claude config documentation
    ├── lesson-guidelines.md   # Detailed guidelines for creating lessons
    ├── lesson-template.html   # Template for new lessons
    └── commands/
        └── new-lesson.md      # Slash command for creating lessons
```

## Design Specifications

### Color Palette

- Primary gradient: `#667eea` → `#764ba2`
- Demo backgrounds: `#e0e7ff`
- Code blocks: `#f5f5f5`

### Typography

- Font: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
- Headings: Purple tones (#667eea, #764ba2)
- Body text: #333

### Layout

- Max width: 900px
- Slide padding: 60px
- Min height: 600px
- Border radius: 20px (container), 10px (elements)

## Browser Compatibility

These lessons work in all modern browsers:

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## Contributing

When adding new lessons:

1. Maintain the established design and structure
2. Ensure all content is in Spanish
3. Include interactive demos when possible
4. Follow the testing checklist
5. Keep lessons self-contained (no external dependencies)

## Future Lesson Ideas

Potential topics for future lessons:

- CSS Position (static, relative, absolute, fixed, sticky)
- CSS Variables (Custom Properties)
- CSS Transitions & Animations
- Advanced CSS Selectors
- Box Model
- Pseudo-elements & Pseudo-classes
- CSS Functions (calc, clamp, var)
- Web Accessibility (ARIA)
- HTML Forms & Validation
- JavaScript Fundamentals
- DOM Manipulation

## License

Educational resource for learning web development fundamentals.

Copyright 2025 Tecnológico de Costa Rica
