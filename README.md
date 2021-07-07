# Frontend Mentor - Huddle landing page with single introductory section solution

This is a solution to the [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)
-




### The challenge

Users should be able to:

- View the optimal layout for the page depending on their device's screen size
- See hover states for all interactive elements on the page





### Links

- Solution URL: (https://youthful-hermann-45417f.netlify.app/)



### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
-Css Animation


### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<h1><main>
      <div class="main-box1 box">
        <div class="box1-text">
          <h3>Grow Together</h3>
          <p>Generate meaningful discussions with your audience and build a strong, loyal community.
            Think of the insightful conversations you miss out on with a feedback form.</p>
        </div>
        <div class="box1-ilustration ilustration">
          <img src="/images/illustration-grow-together.svg" alt="#">
        </div>
      </div>
      <div class="main-box2 box">
        <div class="box2-ilustration ilustration">
          <img src="images/illustration-flowing-conversation.svg" alt="#">
        </div>
        <div class="box2-text">
          <h3>Flowing Conversations</h3>
          <p>You wouldn't paginate a conversation in real life, so why do it online? Our threads
            have just-in-time loading for a more natural flow.</p>
        </div>
      </div>
      <div class="main-box3 box">
        <div class="box3-text">
          <h3>Your Users</h3>
          <p>It takes no time at all to integrate Huddle with your app's authentication solution.
            This means, once signed in to your app, your users can start chatting immediately.</p>
        </div>
        <div class="box3-ilustration ilustration">
          <img src="images/illustration-your-users.svg" alt="#">
        </div>
      </div>
      <div class="main-box4">
        <div>
          <h2>Ready To Build Your Community?</h2>
          <button>Get Started For Free</button>
        </div>
      </div>
    </main></h1>
```
```css
.proud-of-this-css @media (max-width: 768px) {
    header {
      background: url(images/bg-hero-mobile.svg) no-repeat;
    }
    .huddle {
      padding: 1rem 1rem;
    }
    .huddle img {
      width: auto;
      height: 1rem;
    }
    .huddle a {
      padding: 0.3rem 1rem;
      font-size: 0.7rem;
    }
    .heading {
      grid-template-columns: 1fr;
      padding: 1rem;
      text-align: center;
    }
    .heading-text {
      margin-bottom: 3rem;
    }
    .heading-text h1 {
      width: auto;
      font-size: 1.7rem;
    }
    .heading-text p {
      width: auto;
    }
    .heading-pic img {
      width: auto;
      height: 14rem;
    }
  
    main {
      margin: 2rem 1rem;
    }
    .box {
      grid-template-columns: 1fr;
      grid-template-rows: auto auto;
      row-gap: 2rem;
      padding: 2rem 1rem;
      text-align: center;
    }
    .box1-ilustration,
    .box3-ilustration {
      grid-column: 1;
      grid-row: 1/2;
    }
    .box1-text,
    .box3-text {
      grid-column: 1;
      grid-row: 2/3;
    }
    .ilustration img {
      width: auto;
      height: 13rem;
    }
    .main-box4 {
      display: grid;
      grid-template-columns: auto;
      grid-template-rows: auto auto;
      padding: 2rem 2rem;
      margin-bottom: -5rem;
    }
    .main-box4 h2 {
      font-size: 1rem;
    }
    .main-box4 button {
      padding: 0.7rem 2rem;
      font-size: 0.7rem;
    }
  
    footer {
      grid-template-columns: 1fr;
      grid-template-rows: auto auto auto auto;
      padding: 8rem 1rem 1rem 1rem;
    }
    .footer-list {
      grid-template-columns: 1fr;
      grid-template-rows: auto auto auto auto;
    }
    .footer-about,
    .footer-contact {
      justify-self: left;
    }
    .footer-about,
    .footer-social {
      margin-top: 2rem;
    }
    .footer-about a,
    .footer-contact a {
      justify-self: left;
      margin-top: 1rem;
      font-size: 1rem;
    }
    .footer-copyright,
    .attribution {
      text-align: center;
    }
    .footer-copyright {
      margin-top: 2rem;
    }
  } 
```
```js
const boxes = document.querySelectorAll('.box')

window.addEventListener('scroll', checkBoxes)

checkBoxes()
function checkBoxes() {
    const triggerBottom = window.innerHeight / 5 * 4

    boxes.forEach(box => {
        const boxTop = box.getBoundingClientRect().top

        if(boxTop < triggerBottom) {
            box.classList.add('show')
        } else {
            box.classList.remove('show')
        }
    })
}
```


### Useful resources

- [Example resource 1](https://www.udemy.com/course/50-projects-50-days) - This helped me for my scroll animation. I really liked this pattern and will use it going forward.
## Author


- Twitter - [@khadeeejah](https://www.twitter.com/khadeeejah)
# huddle-landing-page
