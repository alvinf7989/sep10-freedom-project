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


[Previous](entry05.md) | [Next](entry07.md)

[Home](../README.md)
