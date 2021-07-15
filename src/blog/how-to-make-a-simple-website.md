---
title: Introduction to HTML
description: Basics of HTML
author: Mihir
date: 2021-07-14T16:27:02.458Z
tags:
  - post
  - featured
image: https://images.unsplash.com/photo-1498050108023-c5249f4df085?ixid=MnwxMjA3fDB8MHxzZWFyY2h8OXx8d2Vic2l0ZXxlbnwwfHwwfHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60
---
## What is HTML?

- HTML stands for Hyper-Text Markup Language
- Hyper-Text refers to the hyperlinks
- HTML is the standard markup language for creating Web pages
- HTML describes the structure of a Web page
- HTML files are saved using `.html` or `.htm` extension.

## HTML Page Structure

Things start with the Document Type Declaration (aka *doctype*), a way to tell the browser this is an HTML page, and which version of HTML we are using.

Modern HTML uses this doctype:

```html
<!DOCTYPE html>
```

Then we have the html element, which has an opening and closing tag:

```html
<!DOCTYPE html>
<html>
...
</html>
```

All tags have an opening and closing tag. Except a few self-closing 
tags that don’t need a closing one because they don’t contain anything *in them*.

The closing tag is same as the opening one, but with a `/`.

The `html` starting tag is used at the beginning of the document, right after the document type declaration.

The `html` ending tag is the last thing present in an HTML document.

Inside the `html` element we have 2 elements: `head` and `body`:

```html
<!DOCTYPE html>
<html>
<head>
...
</head>
<body>
...
</body>
</html>
```

Inside `head`, we will have tags that are essential to creating a web page, like the title, the metadata, and internal or external CSS and JavaScript. Mostly things that do not directly appear on the page, but only help the browser display it properly 

Inside `body` we will have the content of the page. The visible stuff.

## The document heading

The `head` tag contains special tags that define the document properties.

It’s always written before the `body` tag, right after the opening `html` tag:

```html
<!DOCTYPE html>
<html>
<head>
...
</head>
</html>
```

Inside `<head>` tag we can have tags like:

- `title`
- `script`
- `link`
- `style`
- `meta`

### The `title` tag

The title tag determines the page title. The title is displayed in the browser, and it’s especially important as it’s one of the key factors for SEO.

```html
<!DOCTYPE html>
<html>
<head>
<title>Your Page Title</title>
</head>
<html>
```

### The `script` tag

This tag is used to add JavaScript into the page.

You can include it inline, using an opening tag, the JavaScript code and then the closing tag:

```html
<script>
...Some JS
</script>
```

Or you can load an external Javascript file using `src` attribute:

```html
<script src="file.js"></script>
```

In modern JavaScript we have an alternative, more performant than keeping the script at the bottom of the page - `defer` attribute:

```html
<script defer src="file.js"></script>
```

## The `link` tag

The `link` tag is used to set relationships between a document and other resources.

It’s mainly used to link an external CSS file to be loaded.

This element has no closing tag.

```html
<!DOCTYPE html>
<html>
<head>
<link href="file.css" rel="stylesheet">
</head>
</html>
```

The `rel` attribute defines the relationship between a linked resource and the current document

### The `style` tag

This tag can be used to add styles into the document, rather than loading an external stylesheet.

```html
<style>
.someCSS{}
</style>
```

### The `meta` tag

Meta tags perform a variety of tasks and they are very, very important.

Especially for SEO.

`meta` elements only have the starting tag.

The most basic one is the `description` meta tag:

```html
<meta name="description" content="A nice page">
```

The `charset` meta tag is used to set the page character encoding. utf-8 in most cases:

```html
<meta charset="utf-8">
```

The viewport meta tag is used to tell the browser to set the page width depending on the device width.

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```