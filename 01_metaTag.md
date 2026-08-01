## Content Inside the `<head>` Tag

The `<head>` contains information **about the webpage**.

This information is **not visible** on the webpage but helps browsers, search engines, and social media understand your website.

Common things inside `<head>`:

- Meta tags
- Page title
- CSS files
- Favicon
- JavaScript files
- SEO information
- Social media information



### 1. `<!DOCTYPE html>`

```html
<!DOCTYPE html>
```

Tells the browser this document uses **HTML5**.



### 2. `<html lang="en">`

```html
<html lang="en">
```

The root (main) tag of the webpage.

`lang="en"` tells browsers and search engines that the page language is English.



### 3. `<meta charset="UTF-8">`

```html
<meta charset="UTF-8">
```

Sets the character encoding.

Allows almost every language and emoji to display correctly.

Example:

- English
- বাংলা
- हिन्दी
- 😊

Without this tag, some characters may appear as strange symbols.



### 4. Viewport Meta Tag

```html
<meta
name="viewport"
content="width=device-width, initial-scale=1.0">
```

Makes the website responsive on mobile devices.

### width=device-width

Makes the webpage width equal to the device screen.

### initial-scale=1.0

Opens the webpage at normal zoom (100%).



### 5. `<title>`

```html
<title>My Website</title>
```

Sets the webpage title.

Appears in:

- Browser tab
- Google search results
- Bookmarks



### 6. Meta Description

```html
<meta
name="description"
content="Learn HTML, CSS and JavaScript">
```

Short summary of the webpage.

Search engines often show this below the page title.

Helps users know what the page is about.



### 7. Meta Keywords

```html
<meta
name="keywords"
content="HTML,CSS,JavaScript">
```

Earlier used for SEO.

Today Google ignores this tag.

Rarely used on modern websites.



### 8. Author

```html
<meta
name="author"
content="Babu Das">
```

Shows who created the webpage.

Mostly useful for documentation.



### 9. Refresh

```html
<meta
http-equiv="refresh"
content="10">
```

Automatically refreshes the webpage every 10 seconds.

Commonly used for:

- Dashboards
- Live scores
- Monitoring systems

Not recommended for normal websites.



### 10. CSS File

```html
<link
rel="stylesheet"
href="style.css">
```

Connects an external CSS file to the webpage.


### 11. Favicon

```html
<link
rel="icon"
href="favicon.png">
```

Adds the small icon shown in the browser tab.

 

### 12. JavaScript File

```html
<script
defer
src="script.js">
</script>
```

Connects an external JavaScript file.

`defer` means:

- Download JavaScript while HTML loads.
- Run JavaScript after the HTML is fully loaded.

This is the recommended way.

 

### 13. Theme Color

```html
<meta
name="theme-color"
content="#0d6efd">
```

Changes the browser's address bar color on supported mobile browsers.

 

### 14. Canonical URL

```html
<link
rel="canonical"
href="https://example.com">
```

Tells search engines which URL is the original page.

Helps avoid duplicate content.

 

### 15. Open Graph (OG)

```html
<meta property="og:title">
```

Used by:

- Facebook
- WhatsApp
- LinkedIn
- Discord

Controls how the webpage looks when someone shares the link.

Common tags:

- og:title
- og:description
- og:image
- og:url

 

### 16. Twitter Card

```html
<meta
name="twitter:card">
```

Controls how the webpage looks when shared on X (Twitter).

Common tags:

- twitter:title
- twitter:description
- twitter:image

 

### 17. Robots

```html
<meta
name="robots"
content="index, follow">
```

Gives instructions to search engines.

**index**

Allow search engines to show this page in search results.

**follow**

Allow search engines to follow the links on this page.

 

```html
<meta
name="robots"
content="noindex, nofollow">
```

***noindex***

Do not show this page in search results.

**nofollow**

Do not follow the links on this page.

Used for:

- Login page
- Admin page
- Private page
- Testing page

 