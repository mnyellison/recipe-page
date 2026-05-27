# Frontend Mentor - Recipe page solution

This is a solution to the Recipe page challenge on Frontend Mentor. The goal of this challenge was to build a responsive recipe card component as close as possible to the original design.

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size

### Screenshot

![](./assets/images/screenshot.jpg)

### Links

- Solution URL: https://github.com/mnyellison/recipe-page
- Live Site URL: https://recipe-page-six-pearl.vercel.app/

---

## My process

### Built with

- Semantic HTML5
- CSS custom properties
- CSS Grid
- Mobile-first workflow
- Responsive design

---

### What I learned

During this project, I practiced:

- Creating responsive layouts using a mobile-first approach
- Organizing CSS with custom properties (Design Tokens based on Figma Guidelines)
- Learning that using pure numerical values (multipliers) for `line-height` allows perfect inheritance for child elements
- Mastering advanced list customization and modifying bullet points using the `::marker` pseudo-element
- Overcoming table styling hurdles by using `border-collapse: collapse` and applying padding directly onto `td` elements to create seamless divider lines

Example of CSS variables and table structure used in the project:

```css
:root {
  --font-size-xl: 2.5rem;
  --font-size-base: 1rem;
  --spacing-400: 2rem;
}

header p {
  line-height: 1.5; /* Pure multiplier for safe inheritance */
}

.nutrition-table {
  width: 100%;
  border-collapse: collapse;
  margin-top: var(--spacing-300);
}

.nutrition-table tr {
  border-bottom: 1px solid var(--color-stone-150);
}

.nutrition-table tr:last-child {
  border-bottom: none;
}

.nutrition-table td {
  padding: var(--spacing-150) var(--spacing-400);
}
```

---

### Continued development

In future projects, I want to continue improving:

- Advanced Layouts with Flexbox, pushing alignment tricks further
- Responsive layouts
- CSS organization
- Semantic HTML

---

### Useful resources

- Frontend Mentor

---

### AI Collaboration

I used Gemini during this project to:

- Clarify CSS concepts (like `line-height` calculations)
- Brainstorm layout strategies for horizontal dividers (`<hr>` vs borders)
- Fix structural box-model bugs (such as margin collapse/footer bleed)
- Review my commit history strategy
- Learn best practices for mobile-first development

The AI helped me understand concepts instead of only giving ready-made solutions, acting like an experienced peer reviewer validating my logical structure.

---

## Author

- Frontend Mentor - https://www.frontendmentor.io/profile/mnyellison
- GitHub - https://github.com/mnyellison
