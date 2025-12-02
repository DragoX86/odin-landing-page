# Odin Project Assignment #2 - Landing Page:
This assignment requires me to re-create a web page from scratch, closely following [TheOdinProject](https://www.theodinproject.com)'s design, while demonstrating what I've learned about Flexbox.
![image of TheOdinProject's Landing Page desgin](https://cdn.statically.io/gh/TheOdinProject/curriculum/81a5d553f4073e593d23a6ab00d50eef8620796d/foundations/html_css/project/imgs/01.png)
<!--Required colors & font styles:-->
![iamge of colors and fonts that are required for the Landing Page](https://cdn.statically.io/gh/TheOdinProject/curriculum/02f3babb44a3d30dccdf6ca30283ac64ec02abbd/foundations/html_css/flexbox/project-landing-page/imgs/02.png)


## Challenges I Encountered and How I Solved Them:

### Challenge 1:
Trying to get header-links (one, two, and three) to be aligned in a row centered to the top right

![header-links stuck as a column](./readme-resources/challenge1.png)

#### Solution:
The culprit that prevented the header links from being a row was `<ul>` in index.html, removing it solved the issue.

![The culprit in index.html](./readme-resources/culprit1.png)

#### Result:
![Solution result](./readme-resources/solution1.png)


### Challenge 2:
Trying to put hero main text, hero image, and hero secondary text to align like the odin project's example

![issue](./readme-resources/issue2-1.png)

I put hero `main-text` & `hero-image` in a container, then put the hero `secondary-text` and `sign-up` button below it, I was able to get the result closer to odin's example but the issue is the `hero-image`'s makes a large gap between hero `main-text` and hero `secondary-text`, I think I need to adjust my `<div>` container placement and a few changes to the CSS.

![issue2](./readme-resources/issue2-2.png)


#### Solution:
This is most likely the hardest challenge for this assignment, I had to go back and look at my practice css flexbox exercises, specifically exercise number 5 flex-modal. The issue was my `<div>` placment and my order of html elements was wrong, I had to create two new `<div>` containers, one for all of the hero elements called `hero-content`, and another for `hero-image` called `hero-content-right`. I placed `hero-content-right` below `hero-secondary`, and moved `main-text` above `hero-secondary` container, did a few adjustments to the CSS and that fixed my issue.

#### Result:
![Solution result](./readme-resources/solution2.png)


### Challenge 3:
The `call2action` sign up button keeps stretching and would not be the desired size unless it wrapped below `call2action`'s `secondary-text`.

![issue](./readme-resources/issue3-1.png)

This is what I wanted the button to look like (this is when it wraps):
![issue2](./readme-resources/issue3-2.png)

#### Solution:
I solved the issue by putting `sign-up` button inside a new `<div>` container called `call2action-content-right`, then added new lines of CSS to center it, and that fixed the problem. 

**Note to Self:** Put `<button>` element in it's own `<div>` container when using flexbox.

#### Result:
![Solution result](./readme-resources/solution3.png)