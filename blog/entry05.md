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

## Skills
Now let's get a recap of all the skills that I have acquired

### How To Google
This was my first skill that I acquired on the very first entry. For Part A we were looking for Software products of Cooking and all I could find were web apps. I made two Google Searches and sometimes I didn't go on the first website that popped up. I also learned a few things fromn these searches and resources like how Baking & Pastry Arts is different from Culinary Arts and that it refers to preparing, cooking, or presenting & plating the food service.

### Organization
Organization was my second skill that I put on my second entry and I used organization via bullet points. Bullet points can help me separate my ideas just like the `<hr>` tag. I used this for Parts A & B and these were how I organized these ideas and features.

#### Part A
* <-- This bullet point represents the name of the Google Search
  * <-- This indented bullet point represents the link to the website found from Google Search.
    * <-- This other indented bullet point represents the descriptions for the websites.

#### Part B
* <-- This bullet point represents the invention name
  * <-- This indented bullet point represents the description about the invention.
    * <-- This other indented bullet point represents the ideas for the invention.
      * <-- The second squared bullet point which represents more ideas for the other ideas.

As you can see, I used a lot of indentation with my bullet points. I was also told that I shouldn't include the names of the Google Searches for my Freedom Project as that is "behind-the-scenes".

### Creativity
This was a skill that I put in entry 3 back when I was in Part B of the Freedom Project. In this part, we had to imagine a few products for the future that are related to our topic. And with my creativity, I imagined four devices, two of which have similar names. These products are:

* The auto spinning whisk
  * This is a whisk that spins by itself and has the following features:
    * Can be rechargeable with Type C Charging
    * Or can use two AA batteries
    * Can adjust the speeds 1 to 5 on the whisk
* Fry-o-clock
  * A deep fryer that tells you when the food in the fryer is done cooking.
    * Perfect for those that can’t remember the time
    * Can change the temperature.
    * Active when plugged in
* Mini Oven 2.0
  * A miniature oven like no other with some more features.
    * Can change the temperature of how high the heat should be.
    * Can handle 4 big trays or 8 smaller trays.
    * Bigger than a normal miniature oven, but smaller than a big oven.
    * Works as long as it’s plugged.
    * Works with cupcake trays and others
    * Fast heating feature which is allowed to be usable every 6 hours.
    * Removable tray display
* Freeze-o-clock
  * A mini Freezer that tells you when an item is done freezing
    * Can set the timer or have the following modes
      * Jelly which has the timer set to how long it takes for the jelly to be frozen
      * Frozen Solid which sets the timer to how long for an item to be frozen solid.
      * Ice cream which sets the timer to whenever the ice cream is ready to eat.
    * Has all these features usable at the same time.
    * Also with representation
      * If it’s red, the item isn’t frozen
      * If it’s blue, the item is frozen
      * If it’s blue but it shows a frozen ice block, the item is too frozen
    * Active when plugged in.
    * Adjust the coldness of the freezer.
    * An AI that speaks to you in correlation to the freezer.
    * Can tell you when items are frozen.

But I didn't just think of these features on my own. No, I actually showed my ideas on Slack and some people gave me more ideas to my future products of the Freedom Project. By the way when I said two products had similar names, I meant the Freeze-o-clock and Fry-o-clock.

### Debugging
This skill was the one that I "apparently" put in entry 4, despite not completing the learning log yet. I was able to tinker in more than just the W3Schools website. That's right I was able to practice in FreeCodeCamp and the other sources which were YouTube & MDN Web Docs. Ever since I had my learning log, I have increased my intelligence in my tool, which is "CSS Variables". From just changing one variable value to learning fallback values, this has really upgraded my skill of debugging.

Now we get to the skills that I didn't know that I had during some of my entries. Starting with:

* **Attention to detail** I believe this was a skill that I had used in all of the entries along with my other skills.
* **Communication** During Part B, I shared my ideas and products for the future out on Slack and some people gave me a few more ideas to help enhance by products.

### How To Learn
The Debugging skill isn't the only skill I used while tinkering with my tool because a new skill that I have acquired was how to learn. I used a thing called "LOYO" which meant "Learn In Your Own" and that process was very useful during my learning log. I believe the one file it was _most_ useful for was the YouTube file because I couldn't copy and paste any code there and I had to follow what the video had shown. Now that this is the final entry I have to say a few things. <hr> I am currently working on my plan for this Freedom Project and I could not have been able to do this Freedom Project without these five blog entries. It's astounding how far we have gone from Part A to the process of making a website. Now, I finished my wireframe, which is technically at the Creating part of the Engineering Design Process, Now I just need to finsih my plan and then we get to coding. Welp, I guess this is goodbye. Of course I have to update my `bootstrap-components-practice` `html` file, but this will probably be the last change that will be made. I'm Alvin Frias, and this has been my last blog entry.


[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
