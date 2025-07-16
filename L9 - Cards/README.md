# L10 - Practice Pet Rescue

## Learning Objectives
By the end of this lesson, students will be able to:
- Create attractive card layouts using CSS
- Understand how to structure card components with proper HTML semantics
- Apply hover effects and transitions to enhance user interaction
- Use CSS Grid and Flexbox for card container layouts
- Implement responsive card designs that work on different screen sizes

## What are Cards?
Cards are a popular UI design pattern that groups related information in a visually distinct container. They're commonly used for:
- Product listings
- Blog posts
- User profiles
- Social media posts
- Dashboard widgets

## Key CSS Properties for Cards

### Basic Card Structure
```css
.card {
    background: white;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    padding: 20px;
    margin: 16px;
}
```

### Essential Properties
- **`background`**: Sets the card background color
- **`border-radius`**: Creates rounded corners
- **`box-shadow`**: Adds depth and visual separation
- **`padding`**: Creates internal spacing
- **`margin`**: Creates external spacing between cards

### Advanced Card Features
- **`transition`**: Smooth animations on hover
- **`transform`**: Scale, rotate, or translate effects
- **`overflow: hidden`**: Prevents content from breaking card boundaries
- **`max-width`**: Controls card width for responsive design

## Card Layout Patterns

### 1. Grid Layout (Recommended)
```css
.card-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
}
```

### 2. Flexbox Layout
```css
.card-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
}

.card {
    flex: 1 1 300px;
}
```

## Common Card Components

### Image Cards
- Header image with content below
- Perfect for blog posts or products

### Profile Cards
- Avatar, name, and bio information
- Great for team pages

### Info Cards
- Icon, title, and description
- Ideal for features or services

## Accessibility Best Practices
- Use semantic HTML (`article`, `section`, `header`)
- Include proper heading hierarchy
- Ensure sufficient color contrast
- Add focus states for keyboard navigation
- Use descriptive alt text for images

## Browser Support
Cards using CSS Grid and Flexbox are supported in all modern browsers (IE11+).

## Files in this Lesson
- `L9.html` - Interactive demo with various card types
- `L9-Exercise.html` - Practice creating a card gallery
- `resources/` - Images and assets for the lesson

## Next Steps
After mastering cards, you'll learn about:
- Advanced CSS animations
- Component-based design systems
- CSS frameworks like Bootstrap
- Responsive image techniques
