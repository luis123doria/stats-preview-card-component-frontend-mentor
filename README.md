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

![project-screenshot](images\project-screenshot.png)

### Links

- Solution URL: [GitHub Repository](https://github.com/luis123doria/stats-preview-card-component-frontend-mentor)
- Live Site URL: [GitHub Pages](https://luis123doria.github.io/stats-preview-card-component-frontend-mentor/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

In this project I practiced Flexbox and Grid, since it is the most complicated topic for me when developing websites in HTML5 and CSS3.
I learned a little more about the media queries and how to use it

### Continued development

With each project I feel more prepared, I analyze each component to decide what type of `display` to use.
I'm also learning more and more about media queries and how to use them to apply Mobile First responsive design.

In the same way, I still have many doubts about the media queries that I would like to experiment with in future projects, for example, how to use Mobile First correctly.

Should the Mobile code be written in a media querie, or would the media querie be for other screens such as tablet and desktop?

If not, the code gets longer, but allows you to specify many properties in a detailed way:

#### Case 1

```css
/* General property that does not change on any screen */
.main {
    text-align: center;
    font-size: 2rem;
    color: #fff;
}

/* Media querie for mobile (Mobile First) that modify the display of .main */
@media (max-width: 450px){
    .main {
        display: flex;
        flex-direction: column;
    }
}

/* Media querie for desktop that modify the display of .main */
@media (min-width: 1080px){
    .main {
        display: flex;
        flex-direction: row;
    }
}
```

#### Case 2

```css
/* Media querie for mobile (Mobile First) that modify the display of .main */
@media (max-width: 450px){
    .main {
        text-align: center;
        font-size: 2rem;
        color: #fff;
        display: flex;
        flex-direction: column;
    }
}

/* Media querie for desktop that modify the display of .main */
@media (min-width: 1080px){
    .main {
        text-align: center;
        font-size: 2rem;
        color: #fff;
        display: flex;
        flex-direction: row;
    }
}
```

Is the **case 1** better than the **case 2**? Why?

### Useful resources

- [A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/) and [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This amazing articles helped me to understand Grid and Flexbox.  I'd recommend it to anyone still learning this concept.
- [Duotone Generator](https://duotone.shapefactory.co/) - This website automatically generates the beautiful Duotone filter in any image.

## Author

- Website - [Meralu](https://www.meralu.com)
- Frontend Mentor - [@luis123doria](https://www.frontendmentor.io/profile/luis123doria)
