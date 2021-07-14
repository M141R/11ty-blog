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
### What is HTML?

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