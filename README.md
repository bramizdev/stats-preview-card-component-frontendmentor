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
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![Captura de pantalla 2022-11-03 a las 20 10 21](https://user-images.githubusercontent.com/112894363/199870208-7f7f2284-6f48-4814-b44e-c01a9a55aead.png)
![Captura de pantalla 2022-11-03 a las 20 10 08](https://user-images.githubusercontent.com/112894363/199870216-93f7aff2-8b8f-4ff2-91a1-45c25cab0ea5.png)

### Links

- Solution URL: [https://github.com/bramizdev/stats-preview-card-component-frontendmentor](https://github.com/bramizdev/stats-preview-card-component-frontendmentor)
- Live Site URL: [https://bramizdev.github.io/stats-preview-card-component-frontendmentor](https://bramizdev.github.io/stats-preview-card-component-frontendmentor)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

This was a real challenge to me specially the filter on the image, this is the way I did it, however I'm not sure if this was the correct approach.

```html
    <picture class="card-picture">
      <source
        media="(min-width: 768px)"
        srcset="./images/image-header-desktop.jpg"
       />
      <source
        media="(min-width: 250px)"
        srcset="./images/image-header-mobile.jpg"
      />
      <img
        src="./images/image-header-mobile.jpg"
        alt="an image of a business meeting"
      />
    </picture>
```
```css
    .card-picture img {
      display: block;
      width: 100%;
      height: 100%;
      object-fit: cover;
      mix-blend-mode: multiply;
      opacity: 0.8;
      border-radius: 10px 10px 0 0;
    }

    .card-picture {
      display: block;
      background: var(--color-primary-200);
      border-radius: 10px 10px 0 0;
    }
```
## Author

- Website - [Brayan Miza](https://github.com/bramizdev)
- Frontend Mentor - [@bramizdev](https://www.frontendmentor.io/profile/bramizdev)
