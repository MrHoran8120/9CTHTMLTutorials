# Lesson 6 - CSS Variables

## Overview

Learn how to use CSS Variables (Custom Properties) to manage key colors in your website. This makes your CSS easier to maintain and allows for quick theme changes.

## What are CSS Variables?

CSS Variables let you store values that you can reuse throughout your stylesheet. They're perfect for managing colors consistently across your entire website.

## How to Use CSS Variables

### Step 1: Define Variables
Define your key colors in the `:root` selector:

```css
:root {
  --primary-color: #3498db;
  --secondary-color: #e74c3c;
  --background-color: #ffffff;
  --text-color: #333333;
}
```

### Step 2: Use Variables
Apply the variables using the `var()` function:

```css
body {
  background-color: var(--background-color);
  color: var(--text-color);
}

.header {
  background-color: var(--primary-color);
  color: white;
}

.button {
  background-color: var(--secondary-color);
  color: white;
}
```

## Benefits

- **Easy updates**: Change one value to update colors throughout your site
- **Consistency**: Ensures the same colors are used everywhere
- **Quick themes**: Create different color schemes easily
- **Less repetition**: No need to copy the same hex codes multiple times

## Example: Theme Switching

You can create different themes by overriding variables:

```css
/* Default theme */
:root {
  --primary-color: #3498db;
  --secondary-color: #e74c3c;
}

/* Dark theme */
.dark-theme {
  --primary-color: #2980b9;
  --secondary-color: #c0392b;
  --background-color: #2c3e50;
  --text-color: #ecf0f1;
}
```

## Files in This Lesson

- **L6.html**: Basic example showing CSS variables for colors
- **L6Exercise.html**: Practice exercise to implement CSS variables

## Key Rules

1. Variable names start with `--` (two dashes)
2. Define variables in `:root` for global access
3. Use `var(--variable-name)` to apply them
4. Always provide fallback colors when possible

## Beyond Colors

CSS Variables can also store:
- Font sizes: `--large-text: 1.5rem;`
- Spacing: `--padding-standard: 20px;`
- Border radius: `--border-radius: 8px;`
- Font families: `--main-font: 'Arial', sans-serif;`

CSS Variables make your code more maintainable and professional!
