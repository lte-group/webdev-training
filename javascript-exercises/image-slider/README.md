# Image Slider/Carousel

## Exercise Overview

Create a slideshow that cycles through images with next/previous buttons.

## Objectives

- Manage the current slide index state
- Navigate through an array of images
- Handle edge cases (first/last slide navigation)
- Create smooth transitions between slides
- Implement an interactive UI component

## Key Concepts

- Array indexing
- State management (current slide index)
- Event listeners
- DOM manipulation
- CSS transitions/animations
- Modulo operator for circular navigation

## Features to Implement

1. Display one image at a time
2. Previous button to go to the previous slide
3. Next button to go to the next slide
4. Slide indicators/dots showing which slide is active
5. Optional: Auto-play functionality

## Suggested HTML Structure

```html
<div class="slider-container">
    <button id="prev-btn">‹</button>
    <div class="slider">
        <img id="slider-image" src="" alt="Slider image">
    </div>
    <button id="next-btn">›</button>
    <div class="dots-container" id="dots"></div>
</div>
```

## Tasks

1. Create an array of image URLs (or use placeholder images)
2. Create a variable to track the current slide index
3. Create a function to display the current slide
4. Add event listeners to next/previous buttons
5. Implement logic to handle wraparound (last → first, first → last)
6. Add indicator dots that show which slide is active
7. Make dots clickable to jump to specific slides

## Tips

- Start with `currentIndex = 0`
- Use the modulo operator for circular navigation: `(currentIndex + 1) % images.length`
- For going backward: `(currentIndex - 1 + images.length) % images.length`
- Update the image `src` attribute to change the displayed image
- Add CSS transitions for smooth fade or slide effects
- Consider disabling buttons briefly during transitions

## Example Images Array

```javascript
const images = [
    'https://via.placeholder.com/800x400/FF6B6B/FFFFFF?text=Slide+1',
    'https://via.placeholder.com/800x400/4ECDC4/FFFFFF?text=Slide+2',
    'https://via.placeholder.com/800x400/45B7D1/FFFFFF?text=Slide+3',
    'https://via.placeholder.com/800x400/FFA07A/FFFFFF?text=Slide+4'
];
```

## Extension Challenges

- Add auto-play that advances slides every few seconds
- Add pause/play buttons for auto-play
- Pause auto-play when user hovers over the slider
- Add keyboard navigation (arrow keys)
- Add touch/swipe support for mobile devices
- Add different transition effects (fade, slide, zoom)
- Add thumbnail navigation
- Add captions for each image
- Make the slider responsive
- Add lazy loading for images
- Display multiple slides at once

## CSS Animation Ideas

```css
.slider img {
    transition: opacity 0.5s ease-in-out;
}

.fade-out {
    opacity: 0;
}

.fade-in {
    opacity: 1;
}
```
