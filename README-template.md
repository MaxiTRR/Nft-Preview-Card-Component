# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![](images/Screenshot.png)

### Links

- Solution URL: https://gentle-a36b35.netlify.app/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned
Another fairly simple challenge. Basically copy almost the same code that you made for the QR Code Component challenge, adapting it to the current challenge requirement. Many recommendations from the previous challenge were that I could summarize my html code if I didn't use a lot of wrapper tags, but I found that I couldn't get things to work the way I wanted if I did, and I feel more comfortable this way than wanting to. adding modifications I can make sure things line up right (or close to it) from the start. Something new that I was able to implement this time is to perform the hover effect on other html elements that are not just links or buttons, which turned out to be a bit complicated without using tutorials.


### Continued development
Something with which I am not very satisfied is with the code to perform the hover effect on the image. I had to use the W3Schools Image Hover Overlay example, and yet I still don't quite understand the code I'm using, so it's something I should continue to research and practice on.

```css
.card-img{
    margin: 20px 0 0;
    position: relative;
    background-color: var(--Cyan);
    border-radius: 20px;
}

.card-img-main{
    display: block;
    border-radius: 15px;
    max-width: 280px;
    object-fit:fill;
    opacity: 1;
    transition: .5s ease;
    cursor: pointer;   
}

.card-img-hover{
    transition: .5s ease;
    opacity: 0;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    text-align: center;
    overflow: hidden;
    cursor: pointer;
   
}

.card-img:hover .card-img-main{
    opacity: 0.3;
}

.card-img:hover .card-img-hover{
    opacity: 1;
}
```

## Author

- Frontend Mentor -(https://www.frontendmentor.io/profile/MaxiTRR)
