

# Frontend Mentor - Blog preview card solution

This is a solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page
- View the optimal layout depending on their device's screen size
- See a responsive design without the use of standard Media Queries

### Screenshot

![](assets/images/WhatsApp%20Image%202026-06-29%20at%202.45.10%20PM.jpeg) 
### Links

- Solution URL: [GitHub Repository](https://github.com/eslammo05/blog-preview-card)
- Live Site URL: [Live GitHub Pages](https://eslammo05.github.io/blog-preview-card/)

## My process

### Built with

- Semantic HTML5 markup (e.g., `<main>`, `<figure>`, `<figcaption>`)
- CSS custom properties
- Flexbox (for layout and element alignment)
- Mobile-first workflow
- **Modern CSS Typography** (using `clamp()` for fluid responsive text)
- **Local Font Loading** (using `@font-face`)

### What I learned

During this project, I faced several interesting challenges and learned how to solve them using modern CSS techniques rather than traditional workarounds:

**1. Loading Local Fonts:**
Instead of relying on external links like Google Fonts, I learned how to load a local font file (`.ttf`) directly into my CSS using `@font-face`. This is great for performance and offline availability.

```css
@font-face {
  font-family: "Figtree";
  src: 
    local("Figtree"),
    url("../assets/fonts/Figtree-VariableFont_wght.ttf") format("truetype");
}

```

**2. Fluid Typography (Without Media Queries):**
One of the biggest obstacles was making the font size responsive without writing multiple `@media` rules. I discovered and applied the `clamp()` function, which dynamically scales the font size between a minimum and maximum value based on the viewport width (`vw`).

```css
p {
    /* Minimum 14px, flexible 3vw, Maximum 16px */
    font-size: clamp(0.875rem, 3vw, 1rem); 
}

```

**3. Solid Box Shadow:**
To match the exact design, I had to create a "solid" shadow rather than a soft, blurred one. I learned that setting the `blur-radius` to `0px` in the `box-shadow` property achieves this sharp, retro effect.

```css
main {
    border: 2px solid hsl(0, 0%, 7%);
    box-shadow: 8px 8px 0px hsl(0, 0%, 7%);
}

```

### Continued development

In future projects, I want to continue refining my skills in:

* Exploring more advanced uses of CSS mathematical functions like `calc()`, `min()`, and `max()`.
* Deepening my understanding of Semantic HTML to improve accessibility (a11y).
* Mastering Flexbox alignments for more complex component layouts.


## Author

* GitHub - [@eslammo05](https://github.com/eslammo05)
* Frontend Mentor - [@eslammo05](https://www.frontendmentor.io/profile/eslammo05)

