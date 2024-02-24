# Entry 4
##### 2/12/24

Hello there, and welcome back to another segment of Alvin Frias's blog entries. We are one entry close to being halfway, so let's get started with the content.

## Content

Now for content, we are in the era of choosing a tool for our project. And the tool I chose was CSS Variables. So, CSS Variables are variables that substitute the original element. This can perfectly be useful for other elements like colors when you can't remember what the hex codes are. So you may be asking, "How did you tinker with this tool?". Well first off, I went to the following websites: [W3schools](https://www.w3schools.com/css/css3_variables.asp) and [FreeCodeCamp](https://www.freecodecamp.org/news/what-are-css-variables-and-how-to-use-them/) and I did some tinkering with the first part of learning variables. Keep in mind I could only be able to tinker with this tool on the W3schools website. The FreeCodeCamp can only let me see what the code looks like, but not actually edit it. Here's the following code snippet:

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

This code uses the following `var()` element for two colors and they are used globally. Do you see the root selector that's on the top of the code snippet? That's what makes the CSS variables global. To make a local variable you have to put the `--blue` and/or `--white` variable in the selector they choose the color in. Now I tinkered with this by changing the hex code for the `--white` variable from `#ffffff` to `#000000` which makes black. Another way of tinkering of mine was making a local variable by changing the background color of the button or container from white to a different color and give a new variable with two dashes in the selector rather than the `root` selector. So that is roughly what I learned from CSS Variables, but for a bonus since we are now learning about bootstrap I will talk about the Variables in Media Queries. Media Queries **are** related to bootstrap after all.

```
:root {
  --blue: #1e90ff;
  --white: #ffffff;
}

.container {
  --fontsize: 25px;
}

/* Styles */
body {
  background-color: var(--blue);
}

h2 {
  border-bottom: 2px solid var(--blue);
}

.container {
  color: var(--blue);
  background-color: var(--white);
  padding: 15px;
  font-size: var(--fontsize);
}

@media screen and (min-width: 450px) {
  .container {
    --fontsize: 50px;
  }
}
```
In this code snippet you'll see that there's a local variable in the media query and the `container` class. I can tell because in the `.container` selector on the top, the `fontsize` variable is set to `25px` while the `fontsize` variable variable in the `@media` query is set to `50px`

## Sources
The 2 sources that I used for CSS Variables were [W3schools](https://www.w3schools.com/css/css3_variables.asp) and [FreeCodeCamp](https://www.freecodecamp.org/news/what-are-css-variables-and-how-to-use-them/) and as I said before, only the W3schools website can let me edit the code through the CSS Variables website. If I go to the FreeCodeCamp CSS Variables website it will only let me _see_ the code and preview.

## EDP
I am at the Planning part of the proccess where I plan to use the CSS Variable tool for my Freedom Project. Right now, I use the tool to rise to the next Engineering Design Process which will be the Creating part.

## Skills

### Recap
* How To Google: I used this skill for Part A when I had to search up software and hardware inventions for my Culinary-related Freedom Project.

* Organization: I used this skill for both parts A & B. In part A, I organized my ideas in bullet points like this:
* <-- This bullet point represents the name of the Google Search
  * <-- This indented bullet point represents the link to the website found from Google Search.
    * <-- This other indented bullet point represents the descriptions for the websites.

And in Part B, I organized my ideas also in bullet points like this:
* <-- This bullet point represents the invention name
  * <-- This indented bullet point represents the description about the invention.
    * <-- This other indented bullet point represents the ideas for the invention.
      * <-- The second squared bullet point which represents more ideas for the other ideas.

* Creativity: This was another skill I learned from naming my products in Part B like the O-Clock devices that I thought of back then: Fry-O-Clock & Freeze-O-Clock.

### My New Skill
**Debugging:** Debugging is my new skill as I looked for the tool known as CSS Variables. This was a new skill that I learned because this skill involves tinkering with a tool and by using the websites for CSS Variables, I was able to tinker in the [W3schools](https://www.w3schools.com/css/css3_variables.asp) website by creating my own local and global variables.

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
