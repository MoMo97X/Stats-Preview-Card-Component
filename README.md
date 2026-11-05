# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./screenshot.png)

### Links

- Solution URL: [FrontEnd mentor solution page](https://www.frontendmentor.io/solutions/responsive-state-card-component-q4Yj_R80Hf)
- Live Site URL: [Github pages](https://momo97x.github.io/Stats-Preview-Card-Component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

#### 1.using picture tag element with source tag to handle image's change on each screen.

```html
<picture>
  <!-- 1 -->
  <source
    media="(max-width: 43.5rem)"
    srcset="images/image-header-mobile.jpg"
  />
  <!-- 2 -->
  <source media="(min-width: 48rem)" srcset="images/image-header-desktop.jpg" />
  <img src="images/image-header-mobile.jpg" alt="" aria-hidden="true" />
</picture>
```

#### 2.using clamp function to make responsive behaivar with out @media.

```css
.description {
  font-size: clamp(1rem, 0.5rem + 0.5vw, 1.8rem);
}
```

### Continued development

- Make more flexable grid layout.
- Improving responsiveness behaiver's wihtout @media.

### Useful resources

- [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Values/clamp) - This helped me learn about clamp function and it's use.

## Author

- Website - [Github repo](https://github.com/MoMo97X/Stats-Preview-Card-Component)
- Frontend Mentor - [@muhammedarrujbani](https://www.frontendmentor.io/profile/MoMo97X)
