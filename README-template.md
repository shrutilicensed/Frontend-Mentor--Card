# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshot

##### Desktop view:

![](<./solution%20screenshots/Screenshot%20(270).png>)

##### At 1440px:

![](<./solution%20screenshots/Screenshot%20(272).png>)

##### At 384px:

![](<./solution%20screenshots/Screenshot%20(273).png>)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Desktop first workflow

### What I learned

My biggest hurdle were understanding two things:

- Understanding how width works, ie.., where I need to give width a constant value and where I need to add percentages.
- Difference between pixels and rem, and how to convert pixels to rem.
- Center the card

```css
html {
  /* to make 1 rem= 10px */
  /* 10px/16px=0.625=62.5% */
  font-size: 62.5%;
}

/* predicting a constant width for the card */
.card {
  max-width: 25rem;
}

/* giving the content inside the card percentages */
.qr-img,
.heading,
.content {
  width: 100%;
}

/* center the card using flexbox */
.card-outline {
  display: flex;
  align-content: center;
  justify-content: center;
  height: 100vh;
}
```

### Continued development

I still need more experience to to predict constant values based on the demo I see when no dimensions are given. Also, I need more practical experience to finish tasks like these in less time.

### Useful resources

- [mdn web docs - cards](https://developer.mozilla.org/en-US/docs/Web/CSS/Layout_cookbook/Card) - This helped me for understanding cards.
- [aarticle- converting pixels to rem](https://coryrylan.com/blog/converting-css-pixels-to-rems) - This helped me understand rem and pixels

## Author

- Linkedin - [Shruti Choudhary](www.linkedin.com/in/shruti-choudhary-s0613)
- Frontend Mentor - [@shrutilicensed](https://www.frontendmentor.io/profile/shrutilicensed)

## Acknowledgments

My elder brother really helped me by giving me slight hints so I could grasp the logic behind width.
