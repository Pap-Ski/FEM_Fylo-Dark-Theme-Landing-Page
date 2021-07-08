# Frontend Mentor - Fylo dark theme landing page solution

This is a solution to the [Fylo dark theme landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/fylo-dark-theme-landing-page-5ca5f2d21e82137ec91a50fd). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - Fylo dark theme landing page solution](#frontend-mentor---fylo-dark-theme-landing-page-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [The challenge](#the-challenge)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Useful resources](#useful-resources)
  - [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [https://www.frontendmentor.io/solutions/fylo-dark-theme-landing-page-with-bem-and-sass-N-ly3lzCD](https://www.frontendmentor.io/solutions/fylo-dark-theme-landing-page-with-bem-and-sass-N-ly3lzCD)
- Live Site URL: [https://fem-fylo-dark-theme-landing-page-five.vercel.app/](https://fem-fylo-dark-theme-landing-page-five.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- SASS
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- Learnt and implemented the BEM(Block, Element and Modifier) Naming Methodology.

```html
<section class="testimonials">
  <img src="./images/bg-quotes.png" alt="quotes" class="testimonials__quote" />
  <div class="testimonial">
    <p class="testimonial__statement">
      Fylo has improved our team productivity by an order of magnitude. Since
      making the switch our team has become a well-oiled collaboration machine.
    </p>
    <div class="testimonial__person">
      <img
        src="./images/profile-1.jpg"
        alt="prof1"
        class="testimonial__person__img"
      />
      <p class="testimonial__person__name">
        Satish Patel<br /><span class="testimonial__person__position"
          >Founder & CEO, Huddle</span
        >
      </p>
    </div>
  </div>
</section>
```

- Though the BEM naming may seem insane and a bit nasty, it really helps solve issues dealing with specificity in your CSS, since it involves naming classes only. Also, with the help of SASS, the CSS more become more modularised, hence more organised.

```css
.testimonials {
  margin-bottom: 15em;

  &__quote {
    width: 8%;
  }

  .testimonial {
    background: $testimonialBg;
    border-radius: 0.5em;
    padding: 2em;
    margin-bottom: 2em;

    &__statement {
      font-size: 0.8rem;
      margin-bottom: 1.5em;
    }

    &__person {
      width: 80%;
      display: flex;
      gap: 0.5em;

      &__img {
        border-radius: 50%;
        max-width: 2rem;
      }

      &__name {
        font-size: 0.8rem;
        font-weight: 700;
        line-height: 1.5;

        span {
          font-size: 0.6rem;
          font-weight: 400;
        }
      }
    }
  }
}
```

### Useful resources

- ["You probably need BEM CSS in your life" by DesignCourse ](https://www.youtube.com/watch?v=er1JEDuPbZQ) - This helped understand the use of BEM better.

- [SASS Tutorial for Beginners](https://www.youtube.com/watch?v=_a5j7KoflTs) - Another amazing tutorial from freecodecamp.

## Author

- Frontend Mentor - [@Pap-Ski](https://www.frontendmentor.io/profile/Pap-Ski)
