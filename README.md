# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

This Frontend Mentor Challenge is to create a card that displays a QR code. A figma design file was provided, and I was required to reproduce the design to as near pixel perfection as possible by referencing the design file, extracting the important values, and creating the proper HTML markup.

### Screenshot

![Completed QR Code Component Project Screenshot](./images/screenshot_qr-code-component.png)

### Links

- [My Frontend Mentor Solution](https://your-solution-url.com)
- [Live Site](https://davidstrube.github.io/qr-code-component/)

## My process

My primary goal for this project was to utilize a good workflow. I thoroughly used git and github, utilizing development and production branches, maintaining a good commit history, and raising issues to resolve a bug. Prior to coding, I sketched out the key html elements for the component and jot down key values for things such as color, margins, and box-shadow values. Finally, I utilized BEM as a naming structure, and CSS custom properties to abstract color values. 

### Built with

- CSS custom properties
- Flexbox
- Figma
- Google Fonts

### What I learned

I discovered that since images are inline by default, extra space is automatically inserted below images, even with no margins set. This extra space is for descenders--the parts of a "g" or "y" for example that fall below the main line of text. In my implementation this was creating unwanted space that I would prefer to specify with margin. It was an easy fix:

```css
.qr-code-component__img {
  display: block;
}
```

### Continued development

I used limited CSS custom properties for some abstraction:

```css
.root {
  --color-dark-navy: #1f314f;
  --color-grey: #7d889e;
  --color-light-grey: #d5e1ef;
}
```

With larger projects I would prefer to abstract more values, such as border-radius and box-shadow. For this particular instance it would have been overkill.

## Author

- Frontend Mentor - [@DavidStrube](https://www.frontendmentor.io/profile/DavidStrube)
