# Frontend Mentor - Fylo data storage component solution

This is a solution to the [Fylo data storage component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/fylo-data-storage-component-1dZPRbV5n). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the site depending on their device's screen size

### Screenshot

Desktop
![Desktop](./screenshots/Screenshot%202023-01-16%20at%2022-17-06%20Frontend%20Mentor%20Fylo%20data%20storage%20component.png)

mobile
![Mobile](./screenshots/Screenshot%202023-01-16%20at%2022-31-12%20Frontend%20Mentor%20Fylo%20data%20storage%20component.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [SASS](https://sass-lang.com/) - CSS pre-processor
- [BEM metodology](https://getbem.com/) - Block Element Modifier metodology
- GIT flow metodology

### What I learned

In this challeng i was able to put in practice animations, gitflow, and use position to make the aparience of the elements as closes to the challenge

- animations for the bar, and make it the animation responsive
- use gitflow to have a better control of the proyect, even if i didn't have to redo or go back to differents stage of my code
  -use position to make the layout as closest as the challenge

```scss
.bar {
  width: 80%;
  height: 1.5625rem;
  border-radius: 3.125rem;
  position: relative;
  left: 1.5625rem;
  top: 2.1875rem;
  background-color: $Very-Dark-Blue;
  &__clip {
    position: absolute;
    width: 1.25rem;
    height: 1.25rem;
    border-radius: 50%;
    top: 0.1875rem;
    left: 50%;
    background-color: $Pale-Blue;
  }
  &__content {
    width: 50%;
    height: 1.1875rem;
    position: absolute;
    top: 0.1875rem;
    left: 0.25rem;
    border-radius: 3.125rem;
    background-image: linear-gradient(
      90deg,
      rgba(255, 163, 153, 1) 35%,
      rgba(255, 77, 151, 1) 100%
    );
  }
}

//animations
@keyframes content-expand1 {
  0% {
    width: 0%;
  }
  100% {
    width: 72%;
  }
}

.transition1 {
  animation-name: content-expand1;
  animation-duration: 1.4s;
  animation-iteration-count: 1;
  animation-fill-mode: forwards;
  animation-timing-function: ease-out;
}

@keyframes clip-move1 {
  0% {
    left: 0%;
  }
  100% {
    left: 70%;
  }
}
.clip-move1 {
  animation-name: clip-move1;
  animation-duration: 1.5s;
  animation-iteration-count: 1;
  animation-fill-mode: forwards;
  animation-timing-function: ease-out;
}
```

### Continued development

I need to know how to work in a better way with all the animations, i've problems with the animations, further than that everthing its a matter of time

### Useful resources

- [Responsive Animations](https://css-tricks.com/responsive-animations-for-every-screen-size-and-device/) - This article help me with how to aproch the animations

## Author

- Frontend Mentor - [@AlanLopRey](https://www.frontendmentor.io/profile/AlanLopRey)
