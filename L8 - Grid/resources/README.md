# CSS Grid Resources

This folder contains additional resources and assets for the L8 - Grid lesson.

## Key CSS Grid Properties Reference

### Container Properties
```css
display: grid;
grid-template-columns: 1fr 1fr 1fr;
grid-template-rows: 100px 200px;
grid-template-areas: "header header" "sidebar content";
gap: 20px;
justify-items: center;
align-items: center;
```

### Item Properties
```css
grid-column: 1 / 3;
grid-row: 1 / 2;
grid-area: header;
justify-self: start;
align-self: end;
```

## Common Grid Patterns

### 1. Equal Columns
```css
grid-template-columns: repeat(3, 1fr);
```

### 2. Responsive Auto-fit
```css
grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
```

### 3. Fixed and Flexible
```css
grid-template-columns: 200px 1fr 100px;
```

### 4. Named Areas Layout
```css
grid-template-areas: 
    "header header header"
    "nav main aside"
    "footer footer footer";
```

## Image Sources
All images in the exercise files are sourced from Unsplash.com for educational purposes.

## Grid vs Flexbox Guide

### Use CSS Grid for:
- 2D layouts (rows AND columns)
- Complex positioning
- Overall page structure
- When you need to control both dimensions

### Use Flexbox for:
- 1D layouts (either row OR column)
- Component alignment
- Distributing space along one axis
- When content determines layout

## Browser Support
- Modern browsers: Full support
- Internet Explorer 11: Partial support with -ms- prefix
- Edge 16+: Full support

## Useful Grid Resources
- [CSS Grid Generator](https://cssgrid-generator.netlify.app/)
- [Grid Garden Game](https://cssgridgarden.com/)
- [MDN CSS Grid Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)

## Practice Ideas
1. Recreate your favorite website's layout using Grid
2. Build a photo gallery with different sized images
3. Create a dashboard with various sized widgets
4. Design a magazine-style layout with text wrapping
5. Build a responsive card-based interface
