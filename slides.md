---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /assets/intro.jpg
# some information about your slides (markdown enabled)
title: Software Development | Foundations
info: |
  ## Software Development | Foundations
# apply unocss classes to the current slide
class: text-left
drawings:
  persist: false
transition: slide-left
mdc: true
---

# CSS - part 2/3
Software Development Bootcamp - Circuit Stream
- [ ] Utilize the CSS box model for website development
- [ ] Style text using CSS
- [ ] Utilize classes to change different elements

<div class="abs-br m-6 text-xl">
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
TODO: fill in anchor href above to point to github repo for these slides
- take attendance
- verify previous zoom video uploaded
- I updated my menu repo https://github.com/avcoder/css-temp2
-->

---
transition: slide-left
---

# Summary from Last Class
(4 min)

- To contain a bunch of HTML tags, like `<h1> <p>` together in one element, what container tags can I use?
- Why would I want to contain them?
- Name all 3 ways of applying css styles to an html page? (i.e. two ways are not considered best practice)
- What are the 3 steps in creating an external stylesheet?
- Regarding syntax, how do you declare a CSS rule?
- Every html element can be thought of as what shape? _ _ _ model

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
- Discuss iframe tag
-->

---
transition: slide-left
---

# Fix syntax
(1 min)

````md magic-move {lines: true}
```css
// Identify syntax errors

plates (
  backgroundColor; yellow,
)
```

```css
/* Identify syntax errors */

#plates {
  background-color: yellow;
}
```
````

<!-- 
-->

---
transition: slide-left
---

# Review of some CSS properties
(10 min) Watch codepen.io demo as we go thru some of these
|                                                     |                             |
| --------------------------------------------------- | --------------------------- |
| Box related | `width height margin padding border` |
| Colors | `background-color color`  |
| Typography & text | `font-size font-weight font-family text-align text-decoration` |
| Misc. | ` list-style-type` |
| Layout | `display` |

<!-- 
colors:
- how do hex and rgb work?
- inheritance
- font-weight: specificity
- demonstrate specificity war
- READ: https://css-tricks.com/specifics-on-css-specificity/
-->

---
transition: slide-left
---

# Exercise: Box Model and Text
(30 min)

- Play with: [📦 Box Model Playground](https://plus.tuni.fi/graderW/static/compcs200-spring2023/_static/html/boxmodel.html)
- Goto: https://codepen.io/codevilla/pen/raNxvJV and experiment with:
   - `<p>` styles - i.e. change background, colors, width, height. Use px, %, rem, etc.
   - modify padding
   - create a border with different shapes and colors
   - change margins
   - change alignment
- Attempt to complete all the goals as listed in the codepen CSS comments

More info about [Typography Best Practices](https://www.smashingmagazine.com/2009/08/typographic-design-survey-best-practices-from-the-best-blogs/)

<!-- 
Box Model
- padding all vs padding-top etc.
- Discuss difference between content-box and border-box 
- Discuss good practices when typesetting a website

Codepen
- Create a codepen account if you don't have one
-->

---
transition: slide-left
---

# Inheritance, Cascade, Specificity
(10 min) Watch codepen.io demo as we go thru some of these

|                                                     |                             |
| --------------------------------------------------- | --------------------------- |
| CSS | acronym for Cascading Style Sheets |
| Cascade | What happens to a button's background-color if `.btn` and `.btn-success` change it? |
| Specificity | See [CSS SpeciFISHity](https://cscie12.dce.harvard.edu/lecture_notes/2021-fall/20210921/images/css-specifishity.png) chart |
| Inheritance | [some CSS props](https://stackoverflow.com/questions/5612302/which-css-properties-are-inherited) by default inherit values set on the element's parent |

<!-- 
READ: https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Handling_conflicts
-->

---
layout: image-right
transition: slide-left
image: /assets/indigo.png
backgroundSize: 400px 250px
class: text-left
---

# Exercise: Pseudo-classes
(10 min)

- Pseudo-class `:hover` (see [others](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes))
- Recreate the "Select a store" and "Kobo eBook" hover effects from this [Indigo page](https://www.indigo.ca/en-ca/more-peppa-5-minute-stories-peppa-pig/9781546124184.html)
- Goto: https://codepen.io/codevilla/pen/GgRoQeR and attempt goals found in CSS comments
- Try varying up the selector types (i.e. basic HTML tag selectors, to using classes, to using ids)

<!-- 
- How do you inspect an element with :hover?
-->

---
layout: image-right
transition: slide-left
image: /assets/kevinpowell.png
backgroundSize: 500px 450px
class: text-left
---

# 10 minute break
<br/>

🍦 Cool Tips, Trends and Resources:
- ⊞ [List of Block Elements vs Inline Elements](https://www.w3schools.com/html/html_blocks.asp)
- 🎨 [Color Formats in CSS](https://www.joshwcomeau.com/css/color-formats/)
- ⚠️ [CSS Specificity](https://css-tricks.com/specifics-on-css-specificity/)
- 💪 [Intro to FlexBox](https://www.youtube.com/watch?v=Vj7NZ6FiQvo&list=PLu8EoSxDXHP7xj_y6NIAhy0wuCd4uVdid)
- 🏹 [Flexbox Zombies](https://mastery.games/post/flexboxzombies2/)
- 🆎 [Typography for Developers](https://css-tricks.com/typography-for-developers/)
- ✏︎ [Undraw](https://undraw.co/illustrations)

<!-- 
- remember: take attendance
-->

---
layout: image-right
transition: slide-left
image: /assets/inbox.png
backgroundSize: 300px 400px
class: text-left
---

# Exercise: Types, Classes and IDs
(20 min)

- What is the point of adding classes to elements in an HTML file?
- Recreate inbox found at: https://www.mixfont.com/Yellowtail+Radley
- Modify look of elements with classes/IDs:
https://codepen.io/codevilla/pen/NPWNxQm and attempt goals found in CSS comments

<!-- 
-->

---
transition: slide-left
---

# Exercise: Boxes and Classes
(45 min) Menu html repurposed:

- Download repository https://github.com/avcoder/css-exercise-05
- Use the below mockup and try to replicate as close as you can.  (I've included some basic styles.  Feel free to change it.)

<img src="/assets/mockup.png" alt="mockup">

<!-- 
- Follow:
https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Your_first_website/Styling_the_content
- Cascading
- use
-->

---
transition: slide-left
---

## For homework:

- Apply what you've learned so far to your "Personal Website" assignment (aka Portfolio assignment)
- Google some portfolios and attempt to recreate parts of the page that you like for your assignment.  Here are some samples:
   - https://sharon-yi.com
   - https://www.franckwebpro.com/
   - https://themes.3rdwavemedia.com/devcard/bs5/index.html

<!--
- take attendance
-->
