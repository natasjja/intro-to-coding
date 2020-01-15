# Exercise 1: Intro to HTML

## Key Concepts

Before we get started, let's go over some basic concepts first:
- *HTML* stands for Hypertext Markup Language. This is the language used to create Web pages for display in web browsers.

## What we're going to do
In this practical exercise, we will do the following:
- Open the boilerplate files
- Add new tags to the `index.html` page
- Add an image to the page

## Steps

> Hint: Don't forget to save each time you make changes to a file!

1.  Open VS Code

    * Click File > Open
    * Select the boilerplate folder that contains the HTML and CSS files (this is called the root directory)
    * Click on `index.html` to see the main index (in your file navigator on the left)

2.  On your OS (Mac Finder / Windows Explorer)

    * Open the folder with HTML Boilerplate files on your computer.
    * Right click `index.html` and open with Chrome.
      _(This lets you see the file rendered locally. Refresh to see changes.)_

3.  Add new tags to the page

    * Pop the new tags anywhere inside the `<body>` tag. *Note that all the website tags need to go inside the `<body>` tag.*
    * Enter a big heading on the page using the `<h1>` tag. Example here:
      https://www.w3schools.com/tags/tag_hn.asp
    * Add an unordered list using the `<ul>` tag. Example here: 
      https://www.w3schools.com/tags/tag_ul.asp
    * Add some text into a `<p>` tag. Example here: 
      https://www.w3schools.com/tags/tag_p.asp
    * Try a link to somewhere cool using the `<a>` tag. Example here: 
      https://www.w3schools.com/tags/tag_a.asp

4.  Add an image to the page

    * First, pick an image - one from your phone or computer would be great!
    * If your image has spaces in the name, you want to remove them
      e.g. `My Cool Image.jpg` -> `My-Cool-Image.jpg`
    * Make a folder called `images` by right clicking in your root folder and selecting `New Folder`
    * Now we want to drop our image into the folder called `/images`
    * Now we can embed the image in the page using the `<img>` tag. Example here:
      https://www.w3schools.com/tags/tag_img.asp
    * Note that we need to use a relative path to the image because these files aren't hosted online anywhere yet. Example here:
      https://www.w3schools.com/html/html_filepaths.asp

5. An extra to try

    * Find the `<title>` tag. 
    * Add a title and refresh your page - where does it appear?


> HINT: As you add tags into your code, make sure you keep refreshing the page in Chrome to see your changes come through.

## Code reference

Here's an example of what your HTML code might look like when you've completed the steps above:

```html
<body>
    <main>
        <h1>Natasja Laurie</h1>
       
        <img src="images/me.png">
       
        <p>My name's Natasja and I'm an associate software engineer, music and food lover.</p>
       
        <p>My favorite things are:</p>
        <ul>
          <li>Coding</li>
          <li>Music</li>
          <li>Good food</li>
        </ul>
       
        <p>Some links:</p>
        <a href="http://www.linkedin.com">LinkedIn</a>|
        <a href="http://www.instagram.com">Instagram</a>|
        <a href="http://www.facebook.com">Facebook</a>
    </main>
</body>
```
