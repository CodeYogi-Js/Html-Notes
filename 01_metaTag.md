## HTML `<head>` Notes

This chapter explains everything commonly written inside the `<head>` tag.

The `<head>` contains information **about the webpage**.

This information is **not visible** on the webpage but helps:

- Browsers
- Search engines
- Social media platforms

understand your website correctly.



## Chapter 1 → HTML Document Structure
**`<!DOCTYPE html>`**

```html
<!DOCTYPE html>
```

```html
<!-- Tells the browser this document uses HTML5 -->
```

---

**`<html lang="en">`**

```html
<html lang="en">
```

```html
<!-- Root element of the webpage.
     lang="en" tells browsers and search engines that the page language is English. -->
```


## Chapter 2 → Basic Meta Tags

### Character Encoding

```html
<meta charset="UTF-8">
```

```html
<!-- Sets the character encoding to UTF-8.
     Allows English, Bengali, Hindi, Emoji 😊 and almost every language
     to display correctly.
     Without this, some characters may appear as strange symbols. -->
```



### Viewport

```html
<meta name="viewport"
      content="width=device-width, initial-scale=1.0">
```

```html
<!-- Makes the website responsive on phones and tablets.

     width=device-width
         → Makes the webpage width equal to the device screen width.

     initial-scale=1.0
         → Opens the page at normal zoom (100%). -->
```


## Chapter 3 → Page Title

 `<title>`

```html
<title>DevNest | Learn HTML, CSS, JavaScript & React</title>
```

```html
<!-- The page title.

     Appears:

     ✔ Browser tab

     ✔ Google search results

     ✔ Bookmarks

     ✔ Social sharing -->
```



### Chapter 4 → SEO Tags

## Description

```html
<meta
name="description"
content="Discover helpful articles...">
```

```html
<!-- Short description of the webpage.

     Search engines often show this below the page title.

     Helps users know what the page is about.

     Recommended length:

     around 150-160 characters. -->
```



### Keywords

```html
<meta
name="keywords"
content="technology, web development...">
```

```html
<!-- Old SEO tag.

     Earlier Google used it.

     Today Google ignores it because people abused it by adding
     unrelated keywords.

     Some smaller search engines may still read it. -->
```



### Author

```html
<meta
name="author"
content="Your Name">
```

```html
<!-- Shows who created the webpage.

     Mainly useful for documentation.

     Doesn't improve SEO much. -->
```



### Canonical URL

```html
<link rel="canonical"
href="https://www.devnest.dev/">
```

```html
<!-- Prevents duplicate content problems.

     Tells Google:

     "This is the main/original URL of this page."

     Example:

     example.com

     example.com/

     example.com/index.html

     All may show the same page.

     Canonical tells Google which one should be indexed. -->
```


### Robots
**Index & Follow**

```html
<meta name="robots"
content="index, follow">
```

```html
<!--
robots

    → Gives instructions to search engine crawlers
      (Google, Bing, Yahoo, etc.).

index

    → Allow search engines to store (index) this page
      and show it in search results.

follow

    → Allow search engines to crawl and follow all links
      (<a href="">) on this page.

Used for:

✔ Home page

✔ About page

✔ Blog

✔ Product page

✔ Documentation

This is the most common setting for public websites.

Note:

Google already assumes "index, follow" by default,
so this tag is optional unless you want to be explicit.
-->
```

### Noindex & Nofollow

```html
<meta name="robots"
content="noindex, nofollow">
```

```html
<!--
robots

noindex

    → Do NOT store (index) this page.

      The page should not appear in Google or other
      search engine results.

nofollow

    → Do NOT follow any links on this page.

      Search engines will not crawl the links found here.

Used for:

❌ Login page

❌ Admin dashboard

❌ Private pages

❌ Thank-you page after form submission

❌ Internal testing pages

This keeps private or unimportant pages out of search
results and tells search engines not to use the links
on the page for crawling.
-->
```



## Chapter 5 → CSS, Icons & JavaScript

### CSS

```html
<link
rel="stylesheet"
href="./css/01_color.css">
```

```html
<!-- Connects external CSS file to style the webpage. -->
```



### Favicon

```html
<link
rel="icon"
type="image/png"
href="https://cdn-icons-png.flaticon.com/512/10473/10473683.png">
```

```html
<!-- Browser tab icon (favicon). -->
```



### External JavaScript

```html
<script
defer
src="./JavaScript/script.js">
</script>
```

```html
<!-- Loads external JavaScript.

     defer means:

     1. Download JS while HTML is loading.

     2. Execute JS only after HTML is completely parsed.

     Best practice for most websites. -->
```

## Chapter 6 → Mobile Support

### Theme Color

```html
<meta
name="theme-color"
content="#0d6efd">
```

```html
<!-- Changes the browser's UI color on supported mobile browsers.

     Mainly visible in Android Chrome.

     Makes the browser address bar match your website theme. -->
```


### Refresh

```html
<meta
http-equiv="refresh"
content="10">
```

```html
<!-- Automatically refreshes the webpage every 10 seconds.

     Mostly used for dashboards, live score pages,
     monitoring systems, etc.

     NOT recommended for normal websites because it annoys users
     and can interrupt reading. -->
```

## Chapter 7 → Social Media Meta Tags

These tags control how your webpage looks when someone shares it.

### Open Graph (Facebook, WhatsApp, LinkedIn, etc.)

### og:title

```html
<meta property="og:title">
```

```html
<!-- Title shown when someone shares the webpage. -->
```



### og:description

```html
<meta property="og:description">
```

```html
<!-- Description shown while sharing. -->
```



### og:image

```html
<meta property="og:image">
```

```html
<!-- Thumbnail image shown in social media preview.

     Recommended:

     1200 × 630 pixels. -->
```

### og:url

```html
<meta property="og:url">
```

```html
<!-- The original URL of the webpage being shared. -->
```



### og:type

```html
<meta property="og:type">
```

```html
<!-- Defines the type of content.

website

article

profile

video.movie

music.song

etc. -->
```


## Twitter / X Card

### twitter:card

```html
<meta name="twitter:card">
```

```html
<!-- Tells Twitter to use a large image preview. -->
```



### twitter:title

```html
<meta name="twitter:title">
```

```html
<!-- Twitter share title. -->
```



### twitter:description

```html
<meta name="twitter:description">
```

```html
<!-- Twitter share description. -->
```



### twitter:image

```html
<meta name="twitter:image">
```

```html
<!-- Image displayed in Twitter/X share preview. -->
```

### twitter:url

```html
<meta name="twitter:url">
```

```html
<!-- URL used when sharing on Twitter/X. -->
```

### [⬅️ Previous](https://github.com/CodeYogi-Js/Html-Notes)

 