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

![Screenshot of completed design](./design/Screenshot%20of%20completed%20Frontend%20Mentor%20Fylo%20data%20storage%20component.png)

### Links

- Solution URL: [GitHub Repository](https://github.com/Ankia-Fuls/fem-fylo-data-storage-component)
- Live Site URL: [GitHub Pages](https://ankia-fuls.github.io/fem-fylo-data-storage-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- SASS Styling
- BEM

### What I learned

This project helped me practice how to position sections relative to other by making use of position absolute and relative, as well as using ::after and borders to create the small triangle at the bottom of the text box displaying how much storage space is left. It was a good exercise in positioning and spacing elements. 

I am proud of the code I used to create the triangle, shown below. Note that this was done using SCSS, so the media query could be nested as shown.

```css
.storage__remaining::after {
        content: "";
        position: absolute;
        right: 0;
        bottom: -1.375rem;

        width: 0;
        height: 0;
        border-left: 0.6875rem solid transparent;
        border-bottom: 0.6875rem solid transparent;
        border-top: 0.6875rem solid white;
        border-right: 0.6875rem solid white;

        display: none;

        @media only screen and (min-width: 62.5rem) {
            display: block;
        }
    }
```

### Continued development

I would like to continue practicing this type of positioning, especially how to make it screenreader friendly. I also used BEM for the first time in this project and would like to continue practicing how to use it.

### Useful resources

- [How to center a relative element](https://stackoverflow.com/questions/6626314/center-an-item-with-position-relative) - This helped to show me how to center an element that has been set as absolute to the center of the relative element.
- [How to create a triangle in CSS](https://css-tricks.com/snippets/css/css-triangle/) - This helped me understand how to use borders to create triangles in CSS.

## Author

- Frontend Mentor - [@Ankia-Fuls](https://www.frontendmentor.io/profile/Ankia-Fuls)
- GitHub - [@Ankia-Fuls](https://github.com/Ankia-Fuls)