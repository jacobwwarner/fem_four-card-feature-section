# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](/design/screenshot.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Block, Element, Modifier (BEM) CSS class naming conventions
- CSS Grid

### What I learned

Adding grid-templates-areas like this to create named layouts for both desktop and mobile views was suprisingly simple and flexible.

```css
.layout-grid {
    --gap: 2rem;

    display: grid;
    grid-auto-columns: 1fr;
    grid-template-areas: 
        'one'
        'two'
        'three'
        'four'
    ;
    gap: var(--gap);
}

@media (min-width: 800px) {
    .layout-grid {
        grid-template-areas:
            '... two ...'
            'one two four'
            'one three four'
            '... three ...'
        ;
    }
}
```

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/en-US/)

## Author

- Website - [Jacob W. Warner](https://www.your-site.com)
- LinkedIn - [@jacobwwarner](https://www.linkedin.com/in/jacobwwarner)
- Frontend Mentor - [@jacobwwarner](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@jacobwwarner](https://www.twitter.com/jacobwwarner)

## Acknowledgments

- ["Responsive layout practice for beginners" by Kevin Powell](https://youtu.be/JFbxl_VmIx0?si=sxSRoNuAab7PudZd)
