# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### Screenshot

![](./screenshot.png)

### Links

- [Solution URL here](https://github.com/lgwarda/recipe-page.git)
- [Live site URL here](https://lgwarda.github.io/recipe-page/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow

### What I learned

1. The rule `td:last-child` targets the last td element in each row, applying the var `(--brown-800)` color only to the numerical values.

```css
/* Table Styles */
table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 20px;
}

th,
td {
  border-bottom: 1px solid var(--stone-150);
  padding: 10px;
  text-align: left;
}

th {
  background-color: var(--stone-150);
}

/* Set color for only the numerical values in the last column */
td:last-child {
  color: var(--brown-800); /* Match the h2 color */
}
```

2. List Styling:

- Used ::before pseudo-elements for better control of bullet points and numbers
- Implemented custom counter for numbered list
- Maintained consistent spacing and alignment

```css
/* Lists */
ul {
    padding-left: 24px;
    margin: 24px 0;
    list-style: none;
}

ul li {
    margin-bottom: 12px;
    padding-left: 12px;
    position: relative;
    color: var(--stone-600);
}

ul li::before {
    content: "•";
    color: var(--brown-800);
    position: absolute;
    left: -12px;
```

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Example resource 1](https://www.example.com) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Frontend Mentor - [@lgwarda](https://www.frontendmentor.io/profile/lgwarda)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
