# HTML Style Guide

## Table of Content

- [Syntax](#syntax)
- [Comments](#comments)
- [Character Encoding](#character-encoding)
- [Attribute Order](#attribute-order)
- [Performance](#performance)
- [Base Code](#code-base)

## Syntax

Use soft tabs with 2 (two) spaces. You can configure your editor for this or using `.editroconfig`.

```html
<!-- Good -->
<nav class="nav">
  <ul class="nav-menu">
    <li class="nav-item">
      <a class="nav-link">

<!-- Bad -->
<nav class="nav">
      <ul class="nav-menu">
            <li class="nav-item">
                  <a class="nav-link">
```

Always use double quotes.

```html
<!-- Good -->
<div class="main">

<!-- Bad -->
<div class='main'>
```

Don't include a `/` in self-closing elements.

```html
<!-- Good -->
<hr>

<!-- Bad -->
<hr />
```

Separate block element by a blank line and agroup the inners block elements.

```html
<!-- Good -->
<ul class="nav-tabs">
    <li>...</li>
    <li>...</li>
    <li>...</li>
    <li>...</li>
</ul>

<div class="tab-content">
    ...
</div>

<!-- Bad -->
<ul class="nav-tabs">

    <li>...</li>

    <li>...</li>

    <li>...</li>

    <li>...</li>

</ul>
<div class="tab-content">
    ...
</div>
```

**[⬆ back to top](#table-of-contents)**

## Comments

Follow this rule to add comments in HTML.

```html
<!-- This is a good example -->
<!-- /Closing a good example -->
```

**[⬆ back to top](#table-of-contents)**

## Character Encoding

Always use UTF-8 for character encoding.

```html
<head>
    <meta charset="UTF-8">
</head>
```

**[⬆ back to top](#table-of-contents)**

## Attribute Order

HTML attributes should be in this order for facilitate the reading.

1. `class`
1. `id`, `name`
1. `data-*`
1. `src`, `for`, `type`, `href`
1. `title`, `alt`
1. `aria-*`, `role`

```html
<a class="..." id="..." data-modal="toggle" href="#">

<input class="form-control" type="text">

<img class="img-rounded" src="..." alt="...">
```

**[⬆ back to top](#table-of-contents)**

## Performance

No need to specify a type when including CSS and JavaScript files as `text/css` and `text/javascript`.

```html
<head>
<!-- Good -->
<link rel="stylesheet" href="assets/css/style.css" />
<script src="scripts.min.js"></script>

<!-- Bad -->
<script src="scripts.min.js" type="text/javascript"></script>
</head>
```

For a better performance, all javascripts files must be at the end of the code. Before closing the `<body>`.

```html
<!-- Good -->
<script src="scripts.min.js"></script>
</body>

<!-- Bad -->
<script src="scripts.min.js"></script>
</head>
<body>
```

Always minify the code in projects only in HTML. Task builders like [Grunt](http://gruntjs.com/) leaves this easier.

```html
<!-- Good -->
<html><head>...</head><body><div class="container">...</div></body></html>

<!-- Bad -->
<html>
    <head>
        ...
    </head>
    <body>
        <div class="container">
            ...
        </div>
    </body>
</html>
```

**[⬆ back to top](#table-of-contents)**

## Base Code

The following code is a HTML base for faster start the projects.

```html
<!DOCTYPE html>
<html lang="en">
<head>

<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<meta name="format-detection" content="telephone=no">
<meta name="viewport" content="width=device-width">

<link rel="shortcut icon" href="assets/img/ico/favicon.ico" />
<link rel="logo" type="image/svg" href="../assets/img/logo/logo.svg" />
<link rel="stylesheet" href="assets/css/style.css" />

<title></title>

</head>
<body>

<!-- Scripts -->
<script src="assets/js/scripts.min.js"></script>

</body>
</html>
```

For give support a olds Internet Explorer...

```html
<!DOCTYPE html>
<!--[if IE]><![endif]-->
<!--[if IE 7 ]>    <html lang="en" class="ie7">    <![endif]-->
<!--[if IE 8 ]>    <html lang="en" class="ie8">    <![endif]-->
<!--[if IE 9 ]>    <html lang="en" class="ie9">    <![endif]-->
<!--[if (gt IE 9)|!(IE)]><!--><html lang="en"><!--<![endif]-->
<head>
...
```

**[⬆ back to top](#table-of-contents)**
