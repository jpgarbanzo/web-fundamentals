---
description: Create a new interactive lesson file following the established template and guidelines
---

You are helping create a new web fundamentals lesson. Follow these steps:

1. **Ask the user for the topic name** if not provided
   - Example: "CSS Position", "Responsive Design", "Box Model"

2. **Read the guidelines**
   - Read `.claude/lesson-guidelines.md` to understand all requirements
   - Read `.claude/lesson-template.html` to get the base structure

3. **Create the lesson file**
   - Use lowercase with hyphens for filename (e.g., `css-position.html`)
   - Copy the structure from `lesson-template.html`
   - Replace all `[TOPIC]` placeholders with the actual topic name
   - Create 10-12 slides following the standard structure:
     - Slide 1: Title slide with emoji and introduction
     - Slide 2: "¿Qué es [Topic]?" with concepts
     - Slides 3-8: Core concepts (one per slide)
     - Slide 9: "Casos de Uso Comunes"
     - Last slide: "¡Domina [Topic]!" with key points

4. **Add topic-specific content**
   - Write clear, educational content in Spanish
   - Include code examples using the `.code` class
   - Create visual demos using the `.demo-container` class
   - Add topic-specific CSS for demonstrations

5. **Follow the style guide**
   - Use the purple color palette (#667eea, #764ba2)
   - Use `.property` class for technical terms
   - Use `.highlight` class for inline code
   - Include interactive examples where possible

6. **Verify consistency**
   - Check that the navigation works
   - Ensure keyboard controls (arrow keys) function
   - Verify the slide counter updates correctly
   - Confirm all content is in Spanish
   - Test that it matches the style of existing lessons

7. **Remind the user to test**
   - Open the file in a browser
   - Navigate through all slides
   - Test keyboard navigation
   - Check responsiveness

After creating the lesson, provide a summary of:
- File created
- Number of slides
- Key topics covered
- Any special demos or features added
