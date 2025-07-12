# Lesson 7 - @Font-face

## Overview

This lesson will show how you can use fonts.google.com to choose and distribute fonts with your website and make sure the site will look just like you expect it to on every device.

We want to make our websites look professional and consistent across all browsers and devices by using custom fonts.

![Font Example Screenshot](screenshot.png)
*Example of custom fonts applied to a webpage using @font-face* 


## Learning Objectives

By the end of this lesson, students will be able to:

- Use Google Fonts to find and integrate web fonts
- Implement `@font-face` declarations for custom fonts
- Apply custom fonts to specific elements
- Understand font loading and fallback strategies
- Ensure consistent typography across all devices

## What is @font-face?

The `@font-face` CSS rule allows you to define custom fonts for use in your web pages. Instead of relying on fonts installed on the user's computer, you can serve font files directly from your website or use web font services like Google Fonts.

## Two Methods of Using Web Fonts

### Method 1: Google Fonts (Recommended for Beginners)

**Step 1:** Visit [fonts.google.com](https://fonts.google.com)

**Step 2:** Choose your font and select the weights you need

**Step 3:** Copy the `<link>` tag to your HTML head:
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
```

**Step 4:** Use the font in your CSS:
```css
body {
    font-family: 'Roboto', sans-serif;
}
```

### Method 2: Custom @font-face (For Local Font Files)

**Step 1:** Place your font file (`.ttf`, `.woff`, `.woff2`) in your project folder

**Step 2:** Define the font using `@font-face`:
```css
@font-face {
    font-family: 'MyCustomFont';
    src: url('my-font.woff2') format('woff2'),
         url('my-font.woff') format('woff'),
         url('my-font.ttf') format('truetype');
    font-weight: normal;
    font-style: normal;
}
```

**Step 3:** Apply the font to elements:
```css
h1 {
    font-family: 'MyCustomFont', serif;
}
```

## Key Concepts

### Font Formats
- **WOFF2**: Best compression, modern browsers
- **WOFF**: Good compression, wider browser support
- **TTF**: Larger files, universal support
- **EOT**: Internet Explorer only (legacy)

### Font Loading Strategy
```css
@font-face {
    font-family: 'MyFont';
    src: url('font.woff2') format('woff2'),
         url('font.woff') format('woff'),
         url('font.ttf') format('truetype');
    font-display: swap; /* Shows fallback font while loading */
}
```

### Fallback Fonts
Always provide fallback fonts in case your custom font fails to load:
```css
h1 {
    font-family: 'Fascinate', serif; /* Custom font with serif fallback */
}
```

## Best Practices

### Performance
- **Limit font weights**: Only load the weights you actually use
- **Use font-display: swap**: Prevents invisible text during font load
- **Preload critical fonts**: Add `<link rel="preload">` for important fonts
- **Choose efficient formats**: Prefer WOFF2 over TTF when possible

### Accessibility
- **Ensure readability**: Custom fonts should be easy to read
- **Test thoroughly**: Check fonts work across different devices
- **Provide fallbacks**: Always include system font fallbacks
- **Consider dyslexia**: Some decorative fonts can be difficult to read

### File Organization
```
project-folder/
├── index.html
├── styles.css
└── fonts/
    ├── my-font.woff2
    ├── my-font.woff
    └── my-font.ttf
```

## Common Font Pairing Strategies

### Contrast Pairing
- **Heading**: Decorative or distinctive font
- **Body**: Clean, readable sans-serif or serif

### Example Combinations
- **Playfair Display** (headings) + **Source Sans Pro** (body)
- **Montserrat** (headings) + **Open Sans** (body)
- **Lora** (headings) + **Roboto** (body)

## Troubleshooting

### Font Not Loading?
1. Check file path is correct
2. Verify font file isn't corrupted
3. Check browser console for errors
4. Ensure CORS settings allow font loading
5. Test with different font formats

### Font Looks Different?
1. Check font-weight specifications
2. Verify you're loading the correct font style
3. Test fallback fonts are working
4. Check for CSS conflicts

## Files in This Lesson

### `L7.html`
- Demonstrates both Google Fonts and custom `@font-face`
- Shows proper implementation of font loading
- Examples of good font pairing

### Practice Exercise
Try implementing both methods:
1. Add a Google Font to your page header
2. Use a custom font file for special elements
3. Ensure proper fallbacks are in place

## Real-World Applications

### When to Use Google Fonts
- Quick prototyping
- Standard web fonts needed
- Don't want to manage font files
- Need reliable cross-browser support

### When to Use Custom @font-face
- Brand-specific fonts
- Unique design requirements
- Better performance control
- Offline functionality needed

## Next Steps

After mastering font loading, you'll be ready for:
- Advanced typography techniques
- Performance optimization
- Responsive font sizing
- CSS font feature settings

## Important Notes

- **License compliance**: Ensure you have rights to use custom fonts
- **File size matters**: Large font files slow page loading
- **Test everywhere**: Fonts render differently across operating systems
- **Accessibility first**: Prioritize readability over style

Typography is fundamental to good web design. Master these font loading techniques to create professional, consistent designs that work everywhere!
