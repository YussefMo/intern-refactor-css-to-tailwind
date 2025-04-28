# Refactoring from CSS to Tailwind CSS

## Overview

As part of my internship (Task 3), I refactored the project’s styling from traditional CSS to Tailwind CSS. This transition aimed to modernize the codebase, improve maintainability, and leverage Tailwind’s utility-first approach for faster UI development.
[Live Demo](https://movie-app-refactor-to-tailwind.netlify.app/)

## Motivation

- **Maintainability:** Tailwind’s utility classes reduce the need for large, monolithic CSS files.
- **Consistency:** Using Tailwind ensures a consistent design system across the project.
- **Rapid Prototyping:** Utility classes allow for quick UI changes without writing custom CSS.

## Refactoring Steps

1. **Installed Tailwind CSS:**
   - Integrated Tailwind via CDN for rapid adoption (see `<script src="https://cdn.tailwindcss.com"></script>` in `index.html`).
2. **Replaced CSS Classes:**
   - Converted existing CSS classes in HTML to Tailwind utility classes.
   - Example: Instead of `.navbar { padding: 1rem; }`, used `p-4` directly in the HTML elements.
3. **Theme Customization:**
   - Extended Tailwind’s default theme in `main.js` to match the project’s color palette and breakpoints.
   - Example: Added custom colors like `main-color`, `text-color`, and `bg-color`.
4. **Removed Unused CSS:**
   - Deprecated or deleted redundant CSS rules from `style.css` as their responsibilities were replaced by Tailwind classes.
5. **Responsive Design:**
   - Utilized Tailwind’s responsive utilities (e.g., `md:`, `sm:`) to ensure the UI adapts to different screen sizes.

## Before and After

- **Before:**
  - Styling handled by custom CSS in `/css/style.css`.
  - Classes were verbose and required manual updates for each change.
- **After:**
  - Styling handled by Tailwind utility classes in HTML.
  - Custom theme and responsive breakpoints defined in Tailwind config (see `main.js`).
  - Minimal custom CSS remains; most styles are now inlined as Tailwind classes.

## Challenges & Improvements

- **Challenge:** Mapping complex or deeply nested CSS selectors to Tailwind equivalents.
- **Improvement:** Codebase is now easier to read, update, and extend. New features can be styled rapidly using Tailwind utilities.

## Maintenance Tips

- Use Tailwind’s utility classes for most styling needs.
- Keep the Tailwind config (`main.js`) updated with any new theme requirements.
- Remove unused CSS to keep the codebase clean.

## For Contributors

- Make UI changes using Tailwind classes in HTML.
- Update the Tailwind config for new colors, fonts, or breakpoints as needed.
- Refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs) for best practices and utility class references.

---

**Task completed as part of Web Masters Internship Task 3: CSS to Tailwind Refactor.**
