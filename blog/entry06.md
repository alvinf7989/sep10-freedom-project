# Entry 6
##### 5/1/24

## Intro
Welp... This is awkward. So, about a month ago, I said that entry 5 was my last blog entry, but turns out there's another blog entry. In this blog entry, I will talk about how I created my website for the Freedom Project.

## Content

Before I made this project I created two wireframes: Mobile & Desktop as well as also filing out my plan and content.
To start, I had to download a basic bootstrap template called Scrolling Nav. This gave me some text and of course a black nav. This is what I needed to start with my website project. Afterwards, I changed up the Nav to have Internal links to Parts A & B. Since, there's two parts for Part A, I made Part A a dropdown menu, so when you click on Part A, you will get internal links to the Software & Hardware parts of Part A. Now that I finished the nav, I added an image on the top, a Creative Commons licensed image. I tried to adjust the image to center by adding the width of 2033 pixels. That is on a desktop as I'm writing this on school right now, but I'll probably finish this on my own computer. Then I put some text which was the title and description of my Freedom Project on the image. The title and description were made with a Kanit font and the text for the nav was an Ubuntu font. You'll see more of these fonts later on. Here was my class called `.head-image`:
```
.head-image {
    background-image: var(--header-img);
    /* width: 2033px; */
    height: 300px;
}
```
See that uncommented width? We'll get to that later.
<hr> Next, I added a green round squared border around the Introduction paragraph in Ubuntu font. This will be the only part of the website that has a small border than the others. I also adjusted the padding and margin for the text to be fully-centered. This will be normal white for now, but wait till we get beyond MVP. <hr> Next up we have Part A: Software. So wht I did was give this an id of "software" to make that an internal link and then I made the description in Oswald font along with the notes that are in Part A: Software. I didn't include my Google Searches because they were "behind-the-scenes"ish. I made the two web apps split into columns and rows and tried to make them stack on each other when seeing the website on mobile. On the left side, you'll see the links and texts in Ubuntu font and on the right side, the notes about these links and web-apps. They are all organized in bullet points from my organization skills. Also the border-size of the rest of the website has changed to make Part A and Part B more big and important. Keep in mind that each one of these borders have different colors despite having the same properties. <hr> Hardware was the same process as software with adding the links on the left and the notes on the right. In fact, to make this mobile-acceptable, I made each of the columns for every single part to stack on each other if on a small width. <hr> Now while Part B is the same process with a pink-border, I laid out my ideas in four columns by adding the titles of the product and the ideas in one box instead of the titels and notes being separated. <hr> After everything was finished I addedsome finishing touches to it. For example, at the end I noticed that the topic that's in the image element is not being responsive when I change to a smaller width. So I had to uncomment out the width size, so the text can be responsive. The image is still not responsive, but that's a beyond MVP issue. Speaking of beyond MVP, since I had time in my Spring Break, I decided to add a linear gradient type of background to one of the divs in the website. Now of course, I used CSS Variables as my tool to help with this freedom project and here was my root:

```
:root {
    --header-text: #fff;
    --border-color: #2ed422;
    --header-img: url(img/culinary-image.jpeg);
    --bg-colour: #11427a;
    --bland-border: black;
    --part-b: #cf30c0;
}
```

And for those that are wondering...

* `--header-text` = White
* `--border-color`(root) = Light-green
* `--border-color`(.light-blu-border) = Light-blue
* `--bg-colour` = Dark-blue
* `--part-b` = Pink
<hr>
Do you notice that the border-color variable has different values. That's because I used my skill of overriding variables to give a value to a different class. Here's the class it was given to:

```
.light-blu-border {
    --border-color: #93e6f1;
}

.light-blu-border {
    border-width: 5px;
    border-style: solid;
    border-color: var(--border-color);
    border-radius: 20px;
    padding: 10px;
    text-align: center;
}
```

## Sources

**Part A: Software**
* [What Is Culinary Arts?](https://hospitalityinsights.ehl.edu/culinary-arts#:~:text=So%2C%20put%20simply%2C%20culinary%20arts,professions%20that%20involve%20food%20service)
* [What Are The Culinary Arts?](https://www.escoffier.edu/blog/culinary-arts/what-are-the-culinary-arts/)
* [Niche.com](https://www.niche.com/colleges/escoffier-school-of-culinary-arts-boulder/#:~:text=The%20chef%20instructors%20do%20their,my%20decision%20to%20attend%20Escoffier!&text=Being%20a%20student%20at%20the,has%20been%20wonderful%20thus%20far)

**Part A: Hardware**
* [Best Kitchen Tablets](https://www.epicurious.com/expert-advice/the-best-tablets-for-the-kitchen-article)
* [Culinary Hill](https://www.culinaryhill.com/cool-kitchen-gadgets/)

These are all the sources that I used in my Freedom Project. As you can see, these sources are also web apps that I used for Part A of my Freedom Project.

## EDP
After the creating part of my freedom project, I of course tested the website to see if it was working and responsive on mobile. (It was) It was also responsive on the computer side. So, basically I'm at the **Testing part** of the Engineering Design Process.

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

### How To Learn
I used a thing called "LOYO" which meant "Learn In Your Own" and that process was very useful during my learning log. I believe the one file it was _most_ useful for was the YouTube file because I couldn't copy and paste any code there and I had to follow what the video had shown.

### Problem Decomposition
Problem Decomposition was a new skil that I acquired because as I was making my Freedom project website, I had a few days to create the divs of each Part, so in a way, it's like breaking my task of creating a whole website into a few smaller tasks for these days of my Spring Break. <hr> Now for Professionalism, I separated the Intro, Software, Hardware, & Part B into different borders, with the Intro having a small border than the other parts. All the Headers were in Ubuntu font and the descriptions were all in Oswald font. Well, except for the Introduction. The title is the only part of the website that has a Kanit font. That's it for the 6th entry and I feel that I will be back for the 7th entry to talk about working beyond MVP. Anyways, thank you for reading the 6th entry of my blog. Bye!

[Previous](entry05.md) | [Next](entry07.md)

[Home](../README.md)
