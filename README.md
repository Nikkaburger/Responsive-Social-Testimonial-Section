# Frontend Mentor - Responsive Social Testimonial section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

  ## Overview

### The challenge

Users should be able to:

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![](./images/screenshot.jpg)

### Links

- Solution URL: (https://github.com/Nikkaburger/Responsive-Social-Testimonial-Section)
- Live Site URL: (https://playful-jelly-13b6b3.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned
I learnt about using different svg images for background on desktop and mobile devices.

```html
<body>
    <div class="container">
        <div class="box">
        <div class="main">
        <h1>
            10,000+ of our users love our products.
        </h1>
        <p class="intro"> We only provide great products combined with excellent customer service. See what our satisfied customers are saying about our services.</p>
        </div>
        <div class="rating">
            <div class="rating1"><div class="icons">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
            </div> 
                <p class="review">Rated 5 Stars in Review</p>
            </div>
            <div class="rating2"><div class="icons">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
            </div> 
                <p class="review">Rated 5 Stars in Report Guru</p>
            </div>
            <div class="rating3"><div class="icons">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
                <img src="./images/icon-star.svg" alt=" " class="icon">
            </div> 
                <p class="review">Rated 5 Stars in BestTech</p>
            </div>
        </div>
        </div>
        <div class="allreview">
        <div class="testimonial1">
            <div class="details">
                <img src="images/image-colton.jpg" alt=" " class="circle"> 
                <div class="about">
                <div class="name">Colton Smith</div>
                <div class="buyer">Verified Buyer</div>
                </div>
            </div>
            <div class="description">" We needed the same printed design as the one we had ordered a week prior. Not only did they find the original order, but we also received it in time. Excellent! "</div>
        </div>
        <div class="testimonial2">
            <div class="details">
                <img src="images/image-irene.jpg" alt=" " class="circle"> 
                <div class="about">
                <div class="name">Irene Roberts</div>
                <div class="buyer">Verified Buyer</div>
                </div>
            </div>
            <div class="description">" Customer service is always excellent and very quick turn around. Completely delighted with the simplicity of the purchase and the speed of delivery. "</div>
        </div>
        <div class="testimonial3">    
            <div class="details">
                <img src="images/image-anne.jpg" alt=" " class="circle"> 
                <div class="about">
                <div class="name">Anne Wallace</div>
                <div class="buyer">Verified Buyer</div>
                </div>
            </div>
            <div class="description">" Put an order with this company and can only praise them for the very high standard. Will definitely use them again and recommend them to everyone! "</div>
        </div>
        </div>
        </div>
</body>
```
```css
html, body{
    font-size: 15px;
    max-width: 1440px;
    margin: 0px;
    font-family: 'League Spartan', sans-serif;
    background: url("../images/bg-pattern-top-desktop.svg"), url("../images/bg-pattern-bottom-desktop.svg");
    background-repeat: no-repeat;
    background-position: top left, bottom -110px right;
    overflow-x: hidden;
}

.container {
    width: 1005px;
    height: 100%;
    justify-content: center;
    align-items: center;
    display: flex;
    flex-direction: column;
    font-size: 15px;
    margin: 80px 150px;
}

.webimage {
    display: flex;
}

.mobileimage {
    display: none;
}

.box {
    width: 1005px;
    display: flex;
    flex-direction: row;
}

.main {
    justify-content: left;
    margin-left: 5px;
    width: 400px;
    flex-direction: column;
    display: flex;
}

h1{
    color: hsl(300, 43%, 22%);
    font-size: 3rem;
    text-align: left;
    font-weight: 700;
}

p, .intro {
    color: hsl(303, 10%, 53%);
    font-size: 16px;
    text-align: left;
    font-weight: 500;
}

.circle {
    width: 30px;
    height: 30px;
    border-radius: 50%;
    float: left;
    margin-left: 10px;
}

.testimonial1 {
    width: 280px;
    height: 120px;
    display: flex;
    flex-direction: column;
    background-color: hsl(300, 43%, 22%);
    border-radius: 10px;
    font-weight: 400;
    padding: 20px;
}

.testimonial2 {
    margin-top: 20px;
    width: 280px;
    height: 120px;
    margin-left: 20px;
    margin-right: 20px;
    display: flex;
    flex-direction: column;
    background-color: hsl(300, 43%, 22%);
    border-radius: 10px;
    font-weight: 400;
    padding: 20px;
}

.testimonial3 {
    margin-top: 40px;
    width: 280px;
    height: 120px;
    display: flex;
    flex-direction: column;
    background-color: hsl(300, 43%, 22%);
    border-radius: 10px;
    font-weight: 400;
    padding: 20px;
}

.allreview {
    width: auto;
    display: flex;
    flex-direction: row;
    padding: 10px;
}

.description {
    display: flex;
    font-weight: 400;
    line-height: 1.2;
    flex-direction: column;
    color: hsl(0, 0%, 100%);
    padding: 10px;
}

.name {
    color: hsl(0, 0%, 100%);
    font-weight: 500;
}

.details {
    display: flex;
    flex-direction: row;
}

.about {
    margin-left: 10px;
}

.rating {
    margin-top: 20px;
    margin-left: 55px;
    width: 440px;
    display: flex;
    flex-direction: column;
    float: right;
    justify-content: right;
    width: 315px;
    height: auto;
    padding: 10px;
}

.rating1 {
    display: flex;
    height: 40px;
    flex-direction: row;
    width: 400px;
    margin-top: 10px;
    padding-left: 10px;
    margin-bottom: 10px;
    background-color: hsl(300, 24%, 96%);
    border-radius: 10px;
}

.rating2 {
    padding-left: 10px;
    height: 40px;
    display: flex;
    flex-direction: row;
    width: 400px;
    margin-left: 60px;
    margin-bottom: 10px;
    background-color: hsl(300, 24%, 96%);
    border-radius: 10px;
}

.rating3 {
    padding-left: 10px;
    display: flex;
    height: 40px;
    flex-direction: row;
    width: 400px;
    margin-left: 120px;
    margin-bottom: 10px;
    background-color: hsl(300, 24%, 96%);
    border-radius: 10px;
}

.icons {
    justify-self: center;
    align-self: center;
    margin-left: 20px;
}

.icon {
    padding-left: 5px;
}

.review {
    color: hsl(300, 43%, 22%);
    font-weight: 700;
    font-size: 16px;
    padding-left: 50px;
}

.buyer {
    color: hsl(0, 0%, 100%);
    font-size: 15px;
    color: hsl(333, 80%, 67%);
}

### Continued development

My focus is on mastering modern web design techniques through continuous learning, experimentation, and a willingness to adapt to the ever-changing web landscape. 
By focusing on responsive design using, HTML5, CSS3, JavaScript, and PHP, to be adequately equipped to create visually stunning and user-friendly websites. Embrace new technologies, stay curious, and push the boundaries of my creativity to unlock endless possibilities in the world of web development. 

### Useful resources

- [#CSSMediaQuery](https://courses.webdevsimplified.com) - This helped me to understand and fix media query for the mobile version of my design, the tutorial was direct and explanatory. I really liked this pattern and will use it going forward.
- [#HTMLFullCourseforBeginners](https://courses.davegray.codes/) - This is an amazing course which helped me finally understand the functionality of #HTML5 tags. I'd recommend it to anyone still learning this concept.
-[#CSSTutorialFullCourseforBeginners](https://courses.davegray.codes/) - This is an amazing course which helped me finally understand CSS tags, syntax and their functionalities. I'd recommend it to anyone still learning this concept.

## Author

- Website - [Oluwaseun Akeju](https://www.fluxverge.com)
- Frontend Mentor - [@nikkaburger](https://www.frontendmentor.io/profile/nikkaburger)
- Twitter - [@fluxverge](https://www.twitter.com/fluxverge)

## Acknowledgments

Special thanks to Almighty God for the completion of this task, my profound gratitude to Dave Gray, Omolade Sunday, Akinola Akeem and Webdevsimplified for their immense contributions.
```
