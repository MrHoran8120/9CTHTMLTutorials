# Lesson 1 - HTML Basics

## Overview

This lesson introduces the fundamental concepts of HTML through a simple webpage about cats. Students will learn basic HTML structure, text formatting, external stylesheets, and linking between pages.

## Learning Objectives

By the end of this lesson, students will understand:

- Basic HTML document structure (`<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`)
- Text formatting with `<p>`, `<b>`, and `<i>` tags
- How to link external CSS stylesheets
- Creating hyperlinks between HTML pages
- Proper use of semantic HTML elements

## Files in This Lesson

### `L1.html`

The main HTML file containing:

- **Paragraph tags (`<p>`)**: Used to structure text content into readable paragraphs
- **Bold tags (`<b>`)**: For making text bold/emphasized
- **Italic tags (`<i>`)**: For italicizing text (used for the scientific name "Felis catus")
- **Hyperlink (`<a href="">`)**: Links to the second page (L1Dog.html)
- **External stylesheet link**: Connects to L1Style.css for styling

### `L1Dog.html`

A second HTML page that demonstrates:

- Page linking and navigation
- How hyperlinks connect multiple pages together

### `L1Style.css`

External CSS file that provides:

- Visual styling for the HTML content
- Separation of content (HTML) from presentation (CSS)
- Introduction to external stylesheet linking

## Key Concepts Covered

### 1. HTML Document Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- Meta information and links -->
</head>
<body>
    <!-- Visible content -->
</body>
</html>
```

### 2. Text Formatting Tags

- `<p>` - Paragraph tag for grouping text
- `<b>` - Bold text for emphasis
- `<i>` - Italic text for styling (scientific names, foreign words)

### 3. External Stylesheet

```html
<link rel="stylesheet" href="L1Style.css">
```

### 4. Hyperlinks

```html
<a href="L1Dog.html">dogs</a>
```

## Activities for Students

1. **Examine the HTML structure** - Look at how the document is organized
2. **Identify text formatting** - Find examples of bold and italic text
3. **Follow the hyperlink** - Click the link to navigate to the second page
4. **View the CSS connection** - See how external styles affect the appearance
5. **Practice editing** - Try changing text content or adding new paragraphs

## Extensions

Students can try:

- Adding more paragraphs about cats
- Creating additional bold or italic text
- Adding more links between pages
- Experimenting with the CSS file to change colors or fonts

## Best Practices Demonstrated

- Proper HTML5 document structure
- Semantic use of formatting tags
- External CSS for styling (separation of concerns)
- Descriptive link text
- Proper file organization and naming

## Next Steps

After completing this lesson, students will be ready to:

- Learn more HTML tags and elements
- Explore CSS styling in greater detail
- Create more complex page layouts
- Add images and multimedia content

---

**Lesson:** L1 - HTML Basics  
**Focus:** Paragraph tags, text formatting, external stylesheets, hyperlinks  
**Difficulty:** Beginner
