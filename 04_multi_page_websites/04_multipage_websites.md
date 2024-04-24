# Multipage Websites

## Computer File Paths

An absolute file path is the full path from root. A relative file path is a path relative to the file you are working in.

Two dots like `../file.docx` means to move up a level relative to the current directory.

A single dot like `./file.docx` means to look in the current directory. Although this can be omitted, for example, you could write `dog.png` but sometimes this doesn't work, so `./` is preferable.

### Exercise

![01_goal](./img/01_goal.png)

See [01_file_paths_exercise.html](./src/01_computer_file_paths/Folder0/01_file_paths_exercise.html)

## Web Pages

Multipage websites may follow a structure like below

```
project
│   index.html
│   about.html
└───assets
    └───images
        │   image1.png
```

### Exercise

Complete the tasks in the code block below

```html
<h1>Welcome to My Website!</h1>
<!-- Add an image of yourself that links to the about page -->
<a href="./public/about.html"
  ><img src="./assets/images/cat.png" alt="cat"
/></a>
<hr />

<!-- Add a link to your contact me page here -->
<a href="./public/contact.html">Contact Me</a>
```

See [02_web_pages.html](./src/02_web_pages/index.html)

## HTML Boilerplate

Just like there is a structure to a formal letter, there is a structure to HTML files. This is known as the boilerplate.

The boilerplate is below, with comments

```html
<!-- Tells the browser the version of HTML the code is written in, below informs HTML version 5 -->
<!DOCTYPE html>
<html lang="en">
  <!-- The head tags contains metadata about the website, not shown to the user -->
  <head>
    <!-- Ensures the charactes on the website render correctly -->
    <meta charset="UTF=8" />
    <!-- The title is what will be displayed in the tab of the browser -->
    <title>My Website</title>
  </head>
  <!-- The body tags contain all the content of the website -->
  <body>
    <h1>Hello World</h1>
  </body>
</html>
```

VSCode has a shortcut for entering boilerplate code. On a blank .html file, typing `!` will prompt the user the paste HTML boilerplate.

The following is returned.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

### Links

[HTML Boilerplate](https://www.theodinproject.com/lessons/foundations-html-boilerplate)

## Portfolio Website

### Exercise

Build a portfolio showing your projects as part of this tutorial.

See [03_portfolio.html](./src/03_portfolio/index.html)

## How to host your website with GitHub

### What is web hosting

Web hosting is the process of making you rwebsite available on the internet. The files and data that create the website need to be a on a web server. The web server is connected to the internet, making it available 24/7. Viewing the website on your laptop, not connected to the internet is known as working locally.

You can host websites through github.

See my html portfolio [here](https://erenmirza.github.io/html-portfolio/)
