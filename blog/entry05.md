# Entry 5
##### 4/8/24

Welp, this is our 5th entry. Which means we are on the last blog entry of the freedom project. Now I know what you're thinking. You're _probably_ thinking, "Oh, but what about entries 6 to 10?" Turns out those were just placeholders for the blog directory. That's fine. I'm okay with changing my `bootstrap-components-practice` `html` file.
## Content

So, in the content section, I'm going to talk about my tool. The tool that I chose for the Freedom Project website was **CSS Variables**. To start off, I created a learning log and put a few files in the tool.

* Two examples from FreeCodeCamp
* Three examples from W3Schools
* Two examples from other sources

I gave myself eight days to complete my Learning Log and I will list them of what I did day-by-day.

### Day 1
This is when I added my first ever file from W3Schools to tinker with. In this file, I put the code to CSS Variables and basically changed one of the `:root` selector's variable values from white to black. Here are my roots: before and after.

#### Before
```
:root {
  --blue: #1e90ff;
  --white: #ffffff;
}
```
#### After
```
:root {
  --blue: #1e90ff;
  --black: #000000;
}
```

This changed the background colors for the `.container` and `.button` class.

### Day 2
This was when I added my very first file from FreeCodeCamp to tinker with. And instead of changing one value of the `:root` selector, I changed two values from blue & white to cyan & green. Here was my root:

```
:root {
    --cyan: #00ffff;
    --green: #6f853a;
  }
```
The variable names said `main-bg-color` which had a blue value and `main-text-color` which had a white value.

### Day 3
On Day 3, I added a second example from FreeCodeCamp. I organized all of the boxes in that example that the preview shows by color. The order was Red,Blue, Green. I also added a little brightness to all the colors as seen on this `root:`
```
:root {
  --light-red: #FF7F7F;
  --light-green: #90EE90;
  --light-blue: #ADD8E6;
  --black: #000000;
}
```

### Day 4
I added a second example from the W3Schools website. The one thing that I learned from this day was that the CSS Variables can work with the `@keyframes`. So what I did was add a variable and its value for what would happen to the button class if it was hovered on. To control that I added this:
```
button:hover {
    animation-name: clique;
    animation-duration: 500ms;
    animation-fill-mode: forwards;
}

@keyframes clique {
    100% {
        background-color: var(--fade-blue);
    }
}
```
That's right! Animation works with the CSS Variables.

### Day 5
On Day 5 was when there was a two-person Shabr Project. This project had us create a website about a Hot Air Balloon Company using what we learned in SEP including Bootstrap components. We used many of those and I thought this was my chance to show off my CSS Variable skills. The colors I used were the following:
```
:root {
    --blue: #1979e6;
    --orange: #ffbf00;
    --red: #ff0048;
    --yellow: #fbed04;
}
```
And the classes and selectors that used these color variables were the following:
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
Yes, I named the blue variable class after a Disney show.

### Day 6
This was when I added my first ever file of the other sources directory. This first file was from a video on YouTube called [CSS Variables Tutorial](https://www.youtube.com/watch?v=sQUB039MG0I). Now in the `:root` there were just global variables at first. That meant these variables applied to all selectors.
```
:root {
        --main-bg-color:#f4f4f4;
        --main-txt-color: #333;
        --container-width: 90%;
        --header-bg-color: #333;
        --header-txt-color: #fff;
    }
```
However, when we get to the `.box` class, you'll see many local variables:
```
.box {
        --box-bg-color: #ddd;
        --box-main-color: #06c;
        --box-padding: 5px 10px;
        --box-shadow-h-offset: 10px;
        --box-shadow-v-offset: 5px;
        --box-shadow-blur-offset: 5px;
        --box-shadow-blur: 5px;
    }
```
This means that any of these variables can **only** work with the box classes. Now, do you notice how the `box-main-color` value is `#06c`? Well, if we look at what's in this `.box p` class...
```
.box p {
    --box-main-color: #555;
    color: var(--box-main-color);
}
```
You'll see that the variable is completely different. This value will only respond in the `.box p` class, overriding the other variable.

### Day 7
It's the 2nd last day and I added my final file from W3Schools about overriding variables. Now this code may be identical to all the other W3Schools examples, but let's look at the local variables in the button class:
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
As you can see the two local variables and their values for blue and yellow in the button selector have overridden the global variables. The blue and yellow global variables have the same value as before by the way.

### Day 8
On the last day, I added another file on the other sources directory. This time, it's from a website called MDN Web Docs. In this source I learned about a type of variable called a fallback values. You see, a fallback value is when you put a variable name inside the `var()` element and the variable doesn't have a property, so you would have to add a value, so the the selector's elements can change to that value.
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
What you see in this code snippet is all of the fallback values because there's no such thing as the `txt-color` variables. After I learned all of this, I was able to use local & global variables along with fallback values and technique of overriding global & local variables. A thing that I didn't mention is that some of the variable names aren't named after colors, they're named after the element they respond to. This made me wonder if I should do that for my Freedom Project website. 

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
