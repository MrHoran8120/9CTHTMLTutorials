# L8 - CSS Grid

## Learning Objectives
By the end of this lesson, students will be able to:
- Understand the fundamentals of CSS Grid layout system
- Create responsive grid layouts using grid containers and grid items
- Use grid template areas to create complex layouts
- Apply grid properties like grid-gap, grid-template-columns, and grid-template-rows
- Build practical layouts like photo galleries, dashboards, and website layouts
- Understand the difference between CSS Grid and Flexbox and when to use each

## What is CSS Grid?
CSS Grid is a powerful 2-dimensional layout system that allows you to create complex layouts with rows and columns. Unlike Flexbox (which is 1-dimensional), Grid can handle both horizontal and vertical alignment simultaneously.

## Key Concepts

### Grid Container vs Grid Items
- **Grid Container**: The parent element with `display: grid`
- **Grid Items**: The direct children of the grid container

### Grid Terminology
- **Grid Lines**: The dividing lines that make up the structure of the grid
- **Grid Tracks**: The space between two adjacent grid lines (rows or columns)
- **Grid Cells**: The space between two adjacent row and column grid lines
- **Grid Areas**: The total space surrounded by four grid lines

## Essential Grid Properties

### Container Properties
```css
.grid-container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr; /* 3 equal columns */
    grid-template-rows: 100px 200px;    /* 2 rows with specific heights */
    gap: 20px;                          /* Space between grid items */
}
```

### Item Properties
```css
.grid-item {
    grid-column: 1 / 3;     /* Span from column 1 to 3 */
    grid-row: 1 / 2;        /* Span from row 1 to 2 */
}
```

## Common Grid Patterns

### 1. Equal Columns
```css
grid-template-columns: repeat(3, 1fr);
```

### 2. Auto-fit Responsive
```css
grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
```

### 3. Mixed Units
```css
grid-template-columns: 200px 1fr 100px;
```

### 4. Named Grid Areas
```css
grid-template-areas: 
    "header header header"
    "sidebar content content"
    "footer footer footer";
```

## Browser Support
CSS Grid is supported in all modern browsers (IE11+ with -ms- prefix).

## When to Use Grid vs Flexbox
- **Use Grid for**: 2D layouts, complex positioning, overall page structure
- **Use Flexbox for**: 1D layouts, component alignment, distributing space

## Files in this Lesson
- `L8.html` - Interactive demo with various grid layouts
- `L8-Exercise.html` - Practice creating grid-based layouts
- `resources/` - Images and assets for the lesson

## Next Steps
After mastering CSS Grid, you'll learn about:
- Advanced Grid techniques
- CSS Subgrid (when widely supported)
- Combining Grid with Flexbox
- CSS Container Queries
