# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](https://cdn.glitch.global/98396ef4-1970-405b-87ae-c3fbaf5a4bc0/overview.png?v=1655733941098)
  - [The challenge](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj)
  - [Screenshot](https://cdn.glitch.global/98396ef4-1970-405b-87ae-c3fbaf5a4bc0/order%20summary.png?v=1655733778401)
  - [Built with](https://www.lambdatest.com/blog/wp-content/uploads/2018/11/JPG-2.jpg)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Challenge was to create pixel-perfect copy of the project from scratch.

### Screenshot

![](https://cdn.glitch.global/98396ef4-1970-405b-87ae-c3fbaf5a4bc0/order%20summary.png?v=1655733778401)

### Links

- Solution URL: [Add solution URL here](https://order-summary-card-solution.glitch.me)
- Live Site URL: [Add live site URL here](https://order-summary-card-solution.glitch.me)

## My process

First, I assembled all the necessary components in the HTML and then I styled it with using CSS.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title></title>
    <link rel="stylesheet" href="/style.css" />
  </head>

  <body>
    <div class="container">
      <div class="wrapper">
        <img
          class="top-image"
          src="https://cdn.glitch.global/98396ef4-1970-405b-87ae-c3fbaf5a4bc0/illustration-hero.svg?v=1655640229838"
        />
        <h1>Order Summary</h1>
        <p class="description">
          You can now listen to millions of songs,<br />
          audiobooks, and podcasts on any device <br />
          anywhere you like!
        </p>
        <div class="flex-container">
          <img
            class="music-icon"
            src="https://cdn.glitch.global/98396ef4-1970-405b-87ae-c3fbaf5a4bc0/icon-music.svg?v=1655640227324"
          />
          <ul>
            <li><p class="list-a">Annual Plan</p></li>
            <li><p class="list-b">$59.99/year</p></li>
          </ul>
          <a href="#" class="change">Change</a>
        </div>
        <button class="click" type="button">Proceed to Payment</button>
        <p class="cancel">Cancel Order</p>
      </div>
    </div>
  </body>
</html>
```

```css
@import url("https://fonts.googleapis.com/css2?family=Outfit:wght@500;700;900&display=swap");

body {
  position: absolute;
  background-position: top;
  background: url(https://cdn.glitch.global/98396ef4-1970-405b-87ae-c3fbaf5a4bc0/pattern-background-desktop.svg?v=1655640232973)
    no-repeat;
  background-color: #e0e8ff;
  background-size: cover;
  height: 100vh;
  width: 100vw;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 auto;
}

.container {
  display: flex;
  height: 697px;
  width: 450px;
  border-radius: 20px;
  justify-content: center;
  background: white;
  box-shadow: 0px 40px 40px -20px rgba(13, 48, 189, 0.151826);
}

.top-image {
  display: flex;
  width: 450px;
  height: 220px;
  border-radius: 20px 20px 0px 0px;
  margin-bottom: 40px;
}

.flex-container {
  display: flex;
  align-items: center;
  flex-direction: row;
  height: 98px;
  width: 354px;
  margin-left: 48px;
  margin-bottom: 32px;
}

h1 {
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 900;
  font-size: 28px;
  line-height: 37px;
  display: flex;
  justify-content: center;
  text-align: center;
  margin-top: 0px;
  margin-bottom: 17px;
  color: #1f2e55;
}

.description {
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 26px;
  color: #717fa6;
  display: flex;
  justify-content: center;
  text-align: center;
  margin-top: 0px;
  margin-bottom: 20px;
}

ul {
  list-style-type: none;
  padding: 0px;
  margin-left: 20px;
}

button {
  background-color: #382ae1;
  border: none;
  padding: 15px 102px;
  text-align: center;
  box-shadow: 0px 20px 20px rgba(56, 42, 225, 0.190291);
  border-radius: 11px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 900;
  font-size: 15px;
  line-height: 20px;
  color: #ffffff;
  cursor: pointer;
}
.click {
  margin-left: 48px;
  margin-right: 48px;
  margin-bottom: 32px;
}

.cancel {
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 900;
  font-size: 15px;
  line-height: 20px;
  color: #717fa6;
  text-align: center;
  cursor: pointer;
  margin: 0 auto;
}

.list-a {
  width: 117.19px;
  height: 21px;
  margin-bottom: 0px;
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 900;
  font-size: 16px;
  line-height: 21px;
  color: #1f2e55;
}

.list-b {
  width: 92px;
  height: 21px;
  margin-top: 6px;
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 21px;
  color: #717fa6;
}
.music-icon {
  margin-left: 24px;
}

a {
  font-family: "Outfit", sans-serif;
  font-style: normal;
  font-weight: 700;
  font-size: 13px;
  line-height: 17px;
  text-decoration-line: underline;
  color: #382ae1;
  padding: 0px;
  /* 50px cuz it's looking better than 68px */
  margin-left: 50px;
}

a:hover {
  text-decoration: none;
}

```

## Author

- Website - [Giorgi Mekantsishvili](https://www.your-site.com)
- Glitch - [Gmekantsis](https://glitch.com/@gmekantsis)
