# Claude Code Configuration

This directory contains guidelines and templates for maintaining consistency across web fundamentals lesson files.

## Files in this Directory

### `lesson-guidelines.md`
Comprehensive documentation for creating new interactive lesson files. This file contains:
- Complete structure and formatting guidelines
- CSS styling standards and color palette
- Content organization patterns
- JavaScript requirements
- Accessibility requirements
- Testing checklist

**When to use**: Read this file before creating any new lesson to ensure consistency with existing lessons (flexbox.html, grid.html, z-index.html, semantic-html.html).

### `lesson-template.html`
A ready-to-use HTML template with all required structure and styling. This file provides:
- Pre-configured slideshow structure with 10 slides
- All required CSS styles
- Complete JavaScript for navigation
- Placeholder content showing the expected format
- Comments indicating where to add custom content

**When to use**: Copy this file as a starting point for any new lesson.

## Quick Start: Creating a New Lesson

1. **Copy the template:**
   ```bash
   cp .claude/lesson-template.html [your-topic].html
   ```

2. **Replace placeholders:**
   - Search for `[TOPIC]` and replace with your topic name
   - Search for `[...]` placeholders and add your content

3. **Customize demos:**
   - Add topic-specific CSS for demonstrations
   - Create interactive examples relevant to your topic

4. **Test thoroughly:**
   - Use the checklist in `lesson-guidelines.md`
   - Verify navigation, responsiveness, and content

5. **Review guidelines:**
   - Check `lesson-guidelines.md` for any specific requirements
   - Ensure consistency with color palette and typography

## Existing Lessons

Current lesson files that follow these guidelines:
- `css-properties.html` - Common CSS Properties (12 slides)
- `css-selectors.html` - CSS Selectors (12 slides)
- `flexbox.html` - CSS Flexbox (10 slides)
- `grid.html` - CSS Grid (10 slides)
- `z-index.html` - Z-Index and Stacking Context (10 slides)
- `responsive-web.html` - Responsive Web Design (12 slides)
- `git-fundamentals.html` - Git Version Control (12 slides)
- `html-structure.html` - HTML Document Structure (12 slides)
- `semantic-html.html` - Semantic HTML Tags (12 slides)

Use these as reference examples when creating new lessons.

## Key Principles

1. **Consistency**: All lessons should look and feel the same
2. **Clarity**: Educational content should be clear and concise
3. **Spanish**: All content must be in Spanish
4. **Interactive**: Include visual demos whenever possible
5. **Self-contained**: Each HTML file should work independently
6. **Accessible**: Follow accessibility best practices

## Need Help?

When creating a new lesson:
1. First, review `lesson-guidelines.md`
2. Copy `lesson-template.html` as your starting point
3. Reference existing lesson files for examples
4. Follow the testing checklist before considering complete

## Maintenance

When updating guidelines or templates:
- Keep both files in sync
- Update this README if new files are added
- Document any breaking changes or new patterns
