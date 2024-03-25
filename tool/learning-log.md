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




<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
