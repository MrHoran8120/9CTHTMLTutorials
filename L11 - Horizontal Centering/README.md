# L11 - Horizontal Centering Methods

## Overview
This lesson demonstrates the 7 main ways to horizontally center elements in CSS, complete with visual examples, code snippets, and pros/cons for each method.

## Methods Covered

### 1. text-align: center
- **Best for:** Inline and inline-block elements
- **Use case:** Text, images, buttons
- **Browser support:** Excellent (all browsers)

### 2. margin: 0 auto
- **Best for:** Block elements with defined width
- **Use case:** Content blocks, containers
- **Browser support:** Excellent (all browsers)

### 3. Flexbox (justify-content: center)
- **Best for:** Modern layouts, responsive design
- **Use case:** Most centering scenarios
- **Browser support:** Good (IE10+)

### 4. CSS Grid (place-items: center)
- **Best for:** Grid layouts, complex positioning
- **Use case:** Advanced layouts
- **Browser support:** Good (IE11+ with prefixes)

### 5. Absolute Position + Transform
- **Best for:** Overlays, positioning over content
- **Use case:** Modals, tooltips, overlays
- **Browser support:** Good (IE9+)

### 6. Absolute Position + Negative Margins
- **Best for:** Legacy browser support
- **Use case:** When exact dimensions are known
- **Browser support:** Excellent (all browsers)

### 7. display: table-cell
- **Best for:** Fallback for older browsers
- **Use case:** When flexbox/grid aren't available
- **Browser support:** Excellent (all browsers)

## Learning Objectives
By the end of this lesson, students will:
- Understand 7 different horizontal centering techniques
- Know when to use each method
- Understand the pros and cons of each approach
- Be able to choose the right method for different scenarios

## Key Takeaways
- **Flexbox** is the modern go-to solution for most centering needs
- **margin: 0 auto** remains excellent for simple block element centering
- **text-align: center** is perfect for inline content
- Different methods work better in different contexts
- Consider browser support requirements when choosing a method

## Files
- `L11.html` - Main demonstration file with all 7 methods
- `README.md` - This documentation file

## Browser Compatibility
All methods demonstrated work in modern browsers. Legacy methods are included for educational purposes and older browser support scenarios.
