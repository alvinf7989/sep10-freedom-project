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

This code uses the following `var()` element for two colors and they are used globally. Do you see the root selector that's on the top of the code snippet? That's what makes the CSS variables global

## Sources
The 2 sources that I used for CSS Variables were [W3schools](https://www.w3schools.com/css/css3_variables.asp) and [FreeCodeCamp](https://www.freecodecamp.org/news/what-are-css-variables-and-how-to-use-them/) and as I said before, only the W3schools website can let me edit the code through the CSS Variables website. If I go to the FreeCodeCamp CSS Variables website it will let me see the code.

## EDP
I am at the Planning part of the proccess where I plan to use the CSS Variable tool for my Freedom Project. Right now, I use the tool to rise to the next Engineering Design Process.

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
