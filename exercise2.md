# Exercise 2: Intro to CSS

## Key Concepts

Before we get started, let's go over some basic concepts first:
- *CSS* stands for Cascading Style Sheets. CSS describes how HTML elements are to be displayed.

## What we're going to do
In this practical exercise, we will do the following:
- Link our CSS to the HTML we wrote for our home page `index.html`
- Wrap our content
- Center our page

## Steps

1. Link our CSS to our HTML file

    * Open your index.html file
    * Between the two `<head>` tags, add the link to your CSS Stylesheet:
        `<link rel="stylesheet" type="text/css" href="css/styles.css">`

2.  Wrap our content

    * Let's add a `<main>` tag around _all the elements_ we've already added inside our document `<body>`.
    * This makes it easier for us to layout our elements. Example here:
      https://www.w3schools.com/tags/tag_main.asp

3.  Let's center our page with CSS

    * In VS Code, open the file called `styles.css` which is inside the `/css` folder.
    * Let's add some new CSS rules to this file.
    * Let's style the `main` tag we added with `max-width`. Don't forget to wrap all your CSS rules inside curly braces like this:
      `main { max-width: 600px; }`
    * Now let's center it using `margin: auto`.
    * For CSS properties that apply to the same selector, you include them all in the same {} curly brackets. So with our example above, the finished CSS looks like this:
      `main { max-width: 600px; margin: auto; }`
    * _Note that it's fine to have CSS in one line for a small amount, but for 3 or more properties it's common to add a new line for each property to make it easier to read. Some people prefer to add a new line regardless to keep your CSS consistent._
    * Try different maximum widths (say 1200px, 500px, 100px), to see what happens to the layout. Example here: 
      https://www.w3schools.com/css/css_max-width.asp

4.  Try some more CSS

    * We'll change the color of our `<h1>` tag.
    * Pick a color from https://htmlcolorcodes.com/color-picker/ or https://www.w3schools.com/cssref/css_colors.asp
    * Apply that color using the `color` property. Example here:  https://www.w3schools.com/cssref/pr_text_color.asp
    * Try changing the background color of the `<body>` to see what happens!
    * If you make it dark, you'll also want to change the text to be light so it shows up.

5.  Have a play
    * What else might you want to style?
    * Add custom fonts? (see notes below)
    * The color of your text in paragraph tags?
    * Add a border to your image?
    * Add a round corner (`border-radius`) to your image?

> Hint: If you have an idea about how you want your page to look but don't know the CSS to style it, ask for help from a neighbor or one of the workshop helpers!

## Color models in web documents

There are several methods to indicate the color you want to style your tag with, including hexadecimal, which looks like `#000000` and RGB / RGBA (which stands for Red, Green, Blue, Alpha) and looks like `rgba(0,0,0,0.5)`. With RGBA, the numbers in your parentheses stand for `(Red, Green, Blue, Alpha)` so `rgba(0,0,0,0.5)` means 0 Red, 0 Green, 0 Blue, and 50% opacity.


## Adding custom fonts to web documents.

1. You can choose a custom font from https://fonts.google.com 

    * Find a font you want to use
    * Click the red + button
    * Open the bar that appeared at the bottom of the page
    * Copy the 'Embed Font' code, e.g
        `<link href="https://fonts.googleapis.com/css?family=Roboto" rel="stylesheet">`
    * Paste the code inside of the `<head>` tags of your index.html

2. You can also use a web-safe font stack. This provides instructions which tells your computer to look for fonts which are already installed, and if the first option isn't available on the client's hard-drive it moves down the list until it finds one that is available.
https://www.cssfontstack.com/


## Code reference

Here's an example of what your CSS code could look like when you've completed the steps above:

```css
body {
    background-image: url(https://st2.depositphotos.com/4521519/10279/v/950/depositphotos_102798858-stock-illustration-seamless-pattern-with-cherry-tree.jpg);
    background-size: cover;
}

main {
    margin: 50px auto;
    text-align: center;
    border: 3px solid rgb(242, 122, 150);
    background-color: white;
    max-width: 40%;
    padding: 40px;
    font-family: 'Roboto';
}

h1 {
    font-family: 'Pacifico';
    font-size: 50px;
    color: rgb(242, 122, 150);
}

img {
    width: 200px;
    border-radius: 50%;
}

p {
    padding: 20px;
}

a {
    padding-right: 5px;
    color: rgb(242, 122, 150);
}
```