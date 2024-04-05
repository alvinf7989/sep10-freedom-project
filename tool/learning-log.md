# Tool Learning Log

Tool: **CSS Variables**

---

2/28/24:
* [W3Schools](https://www.w3schools.com/css/css3_variables.asp) Tinkered with the first example of variables by changing the white element to black. But I can do better. I added a little code snipet on my W3Schools directory called varexample1.md. On the website the preview used to have a white background, but I edited it to have a black background.

Here's what the code snippet used to look like:
```
:root {
  --blue: #1e90ff;
  --white: #ffffff;
}

body { background-color: var(--blue); }

h2 { border-bottom: 2px solid var(--blue); }

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
}

button {
  background-color: var(--white);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}
```
What I changed was the background colors for the `.container` and `button` class, which eres white at first, but I changed it to black.

3/3/24
* [FreeCodeCamp](https://www.freecodecamp.org/news/what-are-css-variables-and-how-to-use-them/) I also tinkered with the first example of FreeCodeCamp's CSS variable example. This was the CSS code in the beginning:

```
:root {
  --main-bg-color: #000080;
  --main-text-color: #fff;
}

body {
  background-color: var(--main-bg-color);
  color: var(--main-text-color);
  text-align: center;
}
```
So, what I did was change the `main-background` and `text-color` from blue & white to cyan & green.

3/11/24
* I organized the boxes by color in the second example of FreeCodeCamp. Here's what the html looked like before:
```
<div class="box-container">
  <div class="box red-box">Box 1</div>
  <div class="box green-box">Box 2</div>
  <div class="box blue-box">Box 3</div>
</div>
<div class="box-container">
  <div class="box blue-box">Box 4</div>
  <div class="box green-box">Box 5</div>
  <div class="box red-box">Box 6</div>
</div>
```

And here's what the CSS looked like before:
```
:root {
  --maroon-red: #800000;
  --dark-green: #013220;
  --navy-blue: #000080;
  --white: #fff;
}

.box-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.box {
  width: 200px;
  height: 100px;
  margin: 10px 0;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 1.2rem;
  color: var(--white);
}

.red-box {
  background-color: var(--maroon-red);
}

.green-box {
  background-color: var(--dark-green);
}

.blue-box {
  background-color: var(--navy-blue);
}
```
So, what I changed was the colors and I organized the boxes in three colors, in the unchanged preview it was disorganized and too dark. Meanwhile, I gave a lighter color and dark text based on what I think makes the example better from Applied Visual Design.

3/18/24
* I have tinkered with the 2nd example of W3Schools by changing two colors and adding a third color. And I also used `@keyframes` for the buttons when you hover and saw if I can use the variables for `@keyframes`, and you can. And then I used `text-align` to fix the positioning of the header. You can see all of these code snippets on the sources.

3/21/24
* I used my tool on the Shabr project by adding a few colors and givng them Variable names. Here's my `root:`
```
:root {
    --blue: #1979e6;
    --orange: #ffbf00;
    --red: #ff0048;
    --yellow: #fbed04;
}
```
And here are the properties that used them:
```
body {
    background-color: var(--orange);
}

.red-background {
    background-color: var(--red);
}

.bluey {
    background-color: var(--blue);
}

.yellow-back {
    background-color: var(--yellow);
}
```

4/3/24
* I watched a YouTube video online on [CSS Variables Tutorial](https://www.youtube.com/watch?v=sQUB039MG0I) and this teached me how to override variables and use local variables. For example, for local variables the video showed this root:

```
:root {
        --main-bg-color:#f4f4f4;
        --main-txt-color: #333;
        --container-width: 90%;
        --header-bg-color: #333;
        --header-txt-color: #fff;
    }
```
And it also showed the `.box` class with a local variable:
```
.box {
        --box-bg-color: #ddd;
        --box-main-color: #06c;
    }
```
The guy in the video even said that the `--box-bg-color` and `--box-main-color` variables can only be used in the `.box` class. Now from overriding variables, I learned that if you put in a local variable in a selector, class or id and change the property of that variable that already has property as a global variable, it will **only** affect the selector, class or id you put the variable in. here's what the `--box-main-color` variable shows for the box class:
```
.box {
  --box-main-color: #06c;
}
```
And here's what the `--box-main-color` value has as the overriding variable in the `.box p` class:
```
.box p {
    --box-main-color: #555;
    color: var(--box-main-color);
}
```

4/4/24
* I added another example from W3Schools about overriding variables and it was neat. The original root showed this at first:
```
:root {
  --blue: #1e90ff;
  --white: #ffffff;
}
```
So, I did a few tweaks to this root and here's what I ended up with:
```
:root {
  --blue: #1e90ff;
  --yellow: #ffff00;
  --fade-blue: #afafff;
}
```
But that's not all because in the button selector I added a local variable inside that overrides another variable. In the example, it showed one overriden blue variable, but I added another yellow variable that overrides by changing the yellow color to an orange-yellow color. here's how the button selector looks after my tweaks:
```
button {
  --blue: #0000ff;
  --yellow: #ffb100;
  background-color: var(--yellow);
  color: var(--blue);
  border: 1px solid var(--blue);
  padding: 5px;
}
```

4/5/24
* I was told that this was the last day of my learning log, so I organized my last three days like this

**Day 1**
* Add a YouTube example to other-sources directory and tinker and type what I learned.

**Day 2**
* Add another example from W3Schools to learn about overriding variables.

**Day 3**
* Add mdn-web-docs example to other-sources directory and learn about fallback values.

But let's get to what I actually did with my tool. So what I did was learn about fallback values. That meant that if you put a variable name inside the `var()` element and the variable doesn't have a property, you would have to add a cvalue, so that way the the selector's elements can change to that value. Here's what I did for my CSS.

```
:root {
    --box-color: #b45bdf;
}

.one {
    --box-color: aquamarine;
    color: var(--txt-color, blue);
  background-color: var(--box-color);
}

.two {
    --box-color: pink;
    color: var(--txt-colore, red);
  background-color: var(--box-color);
}

.three {
    --box-color: green;
    color: var(--txt-colour, #c784e7);
  background-color: var(--box-color);
}

.four {
    color: var(--txt-col0r, white);
    background-color: var(--box-color);
}
```
As shown, you can see that I used both the technique of overriding variables and adding fallback values. I even put the `.four` class on the CSS to show what the global variable would be. Here's the HTML that I put:
```
      <div class="one">
        <p>One</p>
      </div>
      <div class="two">
        <p>Two</p>
      </div>
      <div class="three">
        <p>Three</p>
      </div>
      <div class="four">
        <p>Four</p>
      </div>
```
This is not all that important it just shows different colored rows in text.
<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
