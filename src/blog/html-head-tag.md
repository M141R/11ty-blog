---
title: HTML Head Tag
description: Second Part Of HTML Series
author: Mihir
date: 2021-07-16T10:04:45.682Z
tags:
  - post
  - featured
  - html
image: /assets/blog/html-head-tag.png
---
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

In modern JavaScript we have an alternative, more preformat than keeping the script at the bottom of the page - `defer` attribute:

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