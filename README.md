## What is a Webpage And Website?
<u style="color : red" ><i>A webpage is a single document on the internet that displays content such as text, images, audio, videos, and links. It is usually created using HTML, CSS, and JavaScript.

A website is a collection of one or more related webpages connected through hyperlinks and hosted under a single domain name.</i></u>

## Besic of HTML
HTML was invented by Tim Berners-Lee in 1991. HTML stands for HyperText Markup Language. It is not a programming language, it is a markup language for the web.

### Human analogy:
1. The skeleton of the human body is HTML.
2. The skin of the human body is CSS.
3. The brain of the human body is JavaScript.

### Car analogy:
1. The car's iron body is HTML.
2. The car's color, interior design, and appearance are like CSS.
3. The car's engine is JavaScript.

### HyperText Markup Language means:
- Hyper = links between pages (reference)
    
    Example: Clicking a link from the Home page to the About page.

- Text = data (information)

    Example: Showing a heading or paragraph on a webpage.
  
- Markup = structure using tags

    Example: Tags tell the browser what each content means.
   
- Language = communication method
   
   Example: HTML is a language used to communicate instructions to the browser.

## How to create HTML

HTML file is created with the `.html` extension, like a text file uses the `.txt` extension.

Example:

- `notes.txt` → computer understands it is a text file.
- `index.html` → browser understands it is an HTML webpage file.

The file extension helps the computer and browser easily identify the file type and how to open it.

Earlier, computers had very small memory and storage, so developers also used the short `.htm` extension instead of `.html`.

Both are the same:

- `.html`
- `.htm`

Both extensions are used for HTML files and webpages/projects.

Every project usually starts with `index.html` because browsers and web servers understand index as the default main page of a website. It became an industry standard, so when someone opens a website folder or domain, the browser automatically looks for the `index.html` file first. That is why most web projects start with the name `index.`

Previously, web projects were mainly organized by separate languages like HTML, CSS, and JavaScript files. This worked for small projects, but in large-scale applications it created scalability and file-management problems because related code was spread across many different folders and files.

Now, the industry is moving toward component-based technologies like [react](https://react.dev/). In component-based development, every small UI part is created as a reusable component that contains its own structure, style, and logic together. This makes large projects easier to manage, improves reusability, and keeps project structure more organized and understandable.

## Previous Web Project Structure (Language-based)
projects were separated by languages:
- HTML → structure
- CSS → design
- JavaScript → functionality

```html
project/
│
├── index.html
├── style.css
├── script.js
```

This was good for small projects.
But in big projects, managing files became difficult because related code was separated into many places.

Example: To change one Navbar:

- HTML in one file
- CSS in another file
- JavaScript in another file

Developers had to work in many files for one small feature.

## Modern Component - Based Structure
Now the industry uses component-based technologies like [react](https://react.dev/).
One small reusable UI part with its own HTML, CSS, and JavaScript together.

Example: 
```plaintext
project/
│
├── components/
│   ├── Navbar.jsx
│   ├── Button.jsx
│   └── Card.jsx
```
### Why Learn HTML, CSS, and JavaScript Before React?

React is built on the fundamentals of **HTML, CSS, and JavaScript**. Before learning React, you should understand these three technologies because React uses them internally.

- `HTML` → Creates the structure of a webpage.
- `CSS` → Styles and designs the webpage.
- `JavaScript` → Adds functionality and interactivity.

React is a `JavaScript library`, not a new programming language. It uses `JSX`, which looks like HTML but is actually JavaScript syntax.

Browsers `do not understand JSX directly`. Before the webpage runs, tools like `Babel` convert JSX into normal JavaScript. React then uses JavaScript to create and update HTML elements in the browser.
***Browser understands  HTML, CSS, JavaScript Browser does not understand directly JSX React code***

That is why learning HTML, CSS, and JavaScript first makes React much easier to understand.

## HTML History

HTML was invented by ***Tim Berners-Lee*** in ***1991***.
Since then, HTML has continued to improve with new versions.

**Example :**
- HTML 1.0
- HTML 2.0
- HTML 3.2
- HTML 4.01
- XHTML
- HTML5 (Current Standard)

Today, developers use ***HTML5*** because it is the modern web standard.

### Basic Structure of an HTML Document

```html
<!DOCTYPE html>
<html lang="en">
<head>

</head>
<body>

</body>
</html>
```

### Explanation

1. `<!DOCTYPE html>`

    This tells the browser that the document uses **HTML5**.

    Without this line, the browser may not display the webpage correctly.



2. `<html lang="en">`

    This is the **root (main) tag** of the HTML document.

    Everything in the webpage is written inside this tag.

    `lang="en"` tells the browser and search engines that the webpage language is **English**.

3. `<head>`

    The `<head>` stores information **about the webpage**.

    Users cannot see this information on the webpage.

    Common things inside `<head>`:

    - Title
    - Meta tags
    - CSS files
    - Fonts
    - Favicon
    - JavaScript files

4. `<body>`

    The `<body>` contains everything that users **can see** on the webpage.

    Examples:

    - Heading
    - Paragraph
    - Image
    - Video
    - Button
    - Form
    - Table
    - List

    Everything visible on the webpage is written inside the `<body>` tag.

## Why is the first HTML file usually named `index.html`?

`index.html` is the **main (default) page** of a website.
When someone opens a website, they usually type only the website name.

Example:

```text
https://example.com/
```

The browser sends a request to the web server.

If no file name is given, the web server automatically looks for:

```text
index.html
```

If `index.html` exists, it opens that page. Because of this, `index.html` became the **industry standard** for the first page of a website.

### Why do developers use `index.html`?

- It is the default homepage.
- The web server looks for it automatically.
- Users do not need to type `index.html` in the URL.
- Almost every website uses it.

Example Project:

```text
project/
│
├── index.html
├── about.html
└── contact.html
```

When you open:

```text
https://example.com/
```

The server automatically opens:

```text
index.html
```

So these usually show the same page:

```text
https://example.com/
```

```text
https://example.com/index.html
```

### Important Note

`index.html` is **not required by HTML**.

You can name your file anything:

```text
home.html
main.html
welcome.html
```

These files also work. Developers use `index.html` because web servers automatically open it when no file name is provided.

 ### [Next ➡️](https://github.com/CodeYogi-Js/Html-Notes/blob/main/01_metaTag.md)