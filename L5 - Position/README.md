# Lesson 5 - CSS Position

https://www.youtube.com/embed/lxvnl7dul_M

The above video summarises the lesson. If you can't hear the audio you might need to open the video manually through another video playing app.

## Overview
...existing content...
```
The above video summarises the lesson. If you can't hear the audio you might need to open the video manually through another video playing app.

## Overview

This lesson introduces CSS positioning, one of the most important concepts for controlling element layout and creating complex designs. Students will learn how to use different position values to place elements precisely where they want them, understanding the relationship between parent and child elements, and how positioning affects document flow.

## Position Values
There are five different position values:

- static
- relative
- fixed
- absolute
- sticky

## Static
This is the default positioning value. Elements with `position: static` are positioned according to the normal document flow. The top, right, bottom, left, and z-index properties have no effect on static elements.Static positioned elements are not affected by the top, bottom, left, and right properties.

## Relative

Elements with `position: relative` are positioned relative to their normal position in the document flow. You can use top, right, bottom, and left properties to offset the element from its normal position, but the original space is still reserved.

## Fixed

Elements with `position: fixed` are positioned relative to the **viewport** (browser window). They remain in the same place even when the page is scrolled. This is useful for creating navigation bars, headers, or floating elements.**

## Absolute

Elements with `position: absolute` are positioned relative to their nearest positioned ancestor (any ancestor with position other than static). If no positioned ancestor exists, it's positioned relative to the initial containing block (usually the html element).

## Sticky

Elements with `position: sticky` act like relative positioning until they reach a specified scroll position, then they become fixed. This creates a "sticky" effect, commonly used for navigation headers that stick to the top when scrolling.

## Key Properties
When using positioning (except static), you can control element placement with:

- **top**: Distance from the top edge
- **right**: Distance from the right edge  
- **bottom**: Distance from the bottom edge
- **left**: Distance from the left edge
- **z-index**: Controls stacking order (which element appears on top)

## Common Use Cases

- **Navigation bars**: Use fixed positioning to keep navigation visible while scrolling
- **Overlays and modals**: Use absolute positioning to center content over the page
- **Sticky headers**: Use sticky positioning for section headers that stick while scrolling
- **Fine-tuning layouts**: Use relative positioning for small adjustments

## Files in This Lesson

- **L5 - Position.html**: Interactive demonstration of all position values with visual examples
- **L5Exercise.html**: Hands-on exercises to practice positioning techniques. An element with position: static; is not positioned in any special way; it is always positioned according to the normal flow of the page. 
