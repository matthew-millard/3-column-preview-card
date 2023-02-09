# 3-column-preview-card

Frontend Mentor Challenge - 3 column preview card

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- Page should be responsive.
- See hover states for all interactive elements on the page

### Screenshot

![3-column cars preview card](./Screenshots/Desktop-Screenshot-3-Column-Preview-Card.png)

![3-column cars preview card](./Screenshots/Mobile-Screenshot-3-Column-Preview-Card.png.png)

### Links

- Solution URL: https://matthew-millard.github.io/3-column-preview-card/

## My process

### Built with

- HTML
- CSS
- Grid template areas
- Firefox Developers Tools
- VS Code
- Mobile-first workflow
- BEM

### What I learned

- I have attempted to play a bit of code golf with this challenge. Throughout I kept trying to think ahead as to where I could reuse my classes as much as possible.

- Code I am proud of:
  `.cards {
    position: absolute;
    top: 0;
    left:50%;
    transform: translate(-50%, 0%);
    padding: 2rem 0;
    width: 90%;
    max-width: 400px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 100%;
    grid-template-rows: auto;
    grid-template-areas:
    'sedans'
    'suvs'
    'luxury';
}`

`@media (min-width: 1440px) {
.cards {
position:absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
max-width: 800px;
grid-template-rows: 1fr;
grid-template-columns: repeat(3, 1fr);
grid-template-areas:
'sedans suvs luxury';
}

    .cards__card--sedans {
        border-radius: 7px 0 0 7px;}
    .cards__card--luxury {
        border-radius: 0 7px 7px 0;}

    .content img {
        width: 55px;
        margin: 1rem 0 2rem;
    }
    .content p:first-of-type {
        margin-bottom: 4rem;
    }

}`

### Continued development

- Keep trying to write efficent and readable code.
- Make an effort to add comments in the code.
- Develop a better workflow.

## Author

- Frontend Mentor - [@matthew-millard](https://www.frontendmentor.io/profile/matthew-millard)

- Github - [matthew-millard](https://github.com/matthew-millard)

## Acknowledgments

- Kevin Powell - [@kevinPowell](https://www.kevinpowell.co/)

- CSS-TRICKS - [@ChrisCoyier](https://css-tricks.com/logic-in-css-media-queries/)
