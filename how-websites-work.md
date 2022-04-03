![Background](https://assets.tryhackme.com/room-banners/howthewebworks.png)

<img src="https://tryhackme-images.s3.amazonaws.com/room-icons/5954bb2535bd14dcaf67a94bf9f2dfa7.png" width="200" height="200" align="left">

# How websites work

##### To exploit a website, you first need to know how they are created

##### If you want to check out the room [click here](https://tryhackme.com/room/howwebsiteswork)

#

### Table of Contents

- [How websites work](#how-websites-work)
        - [To exploit a website, you first need to know how they are created](#to-exploit-a-website-you-first-need-to-know-how-they-are-created)
        - [If you want to check out the room click here](#if-you-want-to-check-out-the-room-click-here)
    - [Table of Contents](#table-of-contents)
- [Task 1 How websites work](#task-1-how-websites-work)
    - [What term best describes the side your browser renders a website?](#what-term-best-describes-the-side-your-browser-renders-a-website)
- [Task 2 HTML](#task-2-html)
    - [Let's play with some HTML! On the right-hand side, you should see a box that renders HTML - If you enter some HTML into the box and click the green "Render HTML Code" button, it will render your HTML on the page; you should see an image of some cats](#lets-play-with-some-html-on-the-right-hand-side-you-should-see-a-box-that-renders-html---if-you-enter-some-html-into-the-box-and-click-the-green-render-html-code-button-it-will-render-your-html-on-the-page-you-should-see-an-image-of-some-cats)
    - [One of the images on the cat website is broken - fix it, and the image will reveal the hidden text answer](#one-of-the-images-on-the-cat-website-is-broken---fix-it-and-the-image-will-reveal-the-hidden-text-answer)
    - [Add a dog image to the page by adding another img tag `(<img>)` on line 11. The dog image location is img/dog-1.png](#add-a-dog-image-to-the-page-by-adding-another-img-tag-img-on-line-11-the-dog-image-location-is-imgdog-1png)
- [Task 3 JavaScript](#task-3-javascript)
    - [Click the "View Site" button on this task. On the right-hand side, add JavaScript that changes the demo element's content to "Hack the Planet"](#click-the-view-site-button-on-this-task-on-the-right-hand-side-add-javascript-that-changes-the-demo-elements-content-to-hack-the-planet)
    - [Add the button HTML from this task that changes the element's text to "Button Clicked" on the editor on the right, update the code by clicking the "Render HTML+JS Code" button and then click the button](#add-the-button-html-from-this-task-that-changes-the-elements-text-to-button-clicked-on-the-editor-on-the-right-update-the-code-by-clicking-the-render-htmljs-code-button-and-then-click-the-button)
- [Task 4 Sensitive Data Exposure](#task-4-sensitive-data-exposure)
    - [View the website on this task. What is the password hidden in the source code?](#view-the-website-on-this-task-what-is-the-password-hidden-in-the-source-code)
- [Task 5 HTML Injection](#task-5-html-injection)
    - [View the website on this task and inject HTML so that a malicious link to <http://hacker.com> is shown](#view-the-website-on-this-task-and-inject-html-so-that-a-malicious-link-to-httphackercom-is-shown)

# Task 1 How websites work

### What term best describes the side your browser renders a website?

    Client side

# Task 2 HTML

### Let's play with some HTML! On the right-hand side, you should see a box that renders HTML - If you enter some HTML into the box and click the green "Render HTML Code" button, it will render your HTML on the page; you should see an image of some cats

    No answer needed (just click the completed button)

### One of the images on the cat website is broken - fix it, and the image will reveal the hidden text answer

    HTMLHERO

### Add a dog image to the page by adding another img tag `(<img>)` on line 11. The dog image location is img/dog-1.png

    DOGHTML

# Task 3 JavaScript

### Click the "View Site" button on this task. On the right-hand side, add JavaScript that changes the demo element's content to "Hack the Planet"

    JSISFUN
>     NOTE: the javascript line used to get this results is `document.getElementById("demo").innerHTML = "Hack the Planet";`

### Add the button HTML from this task that changes the element's text to "Button Clicked" on the editor on the right, update the code by clicking the "Render HTML+JS Code" button and then click the button

    No answer needed
>     NOTE: No answer is needed but for the curious out there if you add the line `<button onclick='document.getElementById("demo").innerHTML = "Button Clicked";'>Click Me!</button>` between the line 7 and 8 in the HTML editor you get the same flag as in the prevoius question in this task.

# Task 4 Sensitive Data Exposure

### View the website on this task. What is the password hidden in the source code?

    testpasswd

# Task 5 HTML Injection

### View the website on this task and inject HTML so that a malicious link to <http://hacker.com> is shown

    HTML_INJ3CTION
> NOTE: You can look up how to creat an html link in the <https://www.w3schools.com/html/html_links.asp> site, and don't worry the first example they give on how to create the tag is enough to trigger the correct answer in the room. Just in case this is the line used `<a href="url">link text</a>`
