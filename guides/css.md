# CSS Style Guide

## CSS Summary

- [Syntax](#syntax)
- [Declaration Order](#order)
- [Class Name](#class-name)
- [Performance](#performance)
- [Import](#import)
- [Media Queries](#media-queries)
- [Prefixed properties](#prefixed-properties)
- [Shorthand notation](#shorthand-notation)
- [Pre-Processors](#pre-processors)
- [Comments](#comments)

## Syntax

Use soft tabs with 4 (four) spaces. You can configure your editor for this.


```css
/* Good */
.nav-item {
    display: inline-block;
    margin: 0 5px;
}

/* Bad */
.nav-item {
  display: inline-block;
  margin: 0 5px;
}
```

Always use double quotes.

```css
/* Good */
[type="text"]
[class^="..."]

.nav-item:after {
    content: "";
}

/* Bad */
[type='text']
[class^='...']

.nav-item:after {
    content: '';
}
```

Include a single space before the opening brace of a ruleset.

```css
/* Good */
.header {
    ...
}

/* Bad */
.header{
    ...
}
```

Include a single space after the colon of a declaration.

```css
/* Good */
.header {
    margin-bottom: 20px;
}

/* Bad */
.header{
    margin-bottom:20px;
}
```

Include a semi-colon at the end of the last declaration in a declaration block.

```css
/* Good */
.header {
    margin-bottom: 20px;
}

/* Bad */
.header{
    margin-bottom:20px
}
```

Keep one declaration per line.

```css
/* Good */
.selector-1,
.selector-2,
.selector-3 {
    ...
}

/* Bad */
.selector-1, .selector-2, .selector-3 {
    ...
}
```

Single declarations should remain in one line.

```css
/* Good */
.selector-1 { width: 50%; }

/* Bad */
.selector-1 {
    width: 50%;
}
```

Separate each ruleset by a blank line.

```css
/* Good */
.selector-1 {
    ...
}

.selector-2 {
    ...
}

/* Bad */
.selector-1 {
    ...
}
.selector-2 {
    ...
}
```

Use lowercase, shorthand hex values and avoid specifying units is zero-values.

```css
/* Good */
.selector-1 {
    color: #aaa;
    margin: 0;
}

/* Bad */
.selector-1 {
    color: #AAAAAA;
    margin: 0px;
}
```

**[⬆ back to top](#table-of-contents)**

## Declaration Order

Related property declarations should be grouped together following the order:

```css
.declaration-order {
    /* Position */
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: 100;

    /* Box-model */
    display: block;
    float: right;
    width: 100px;
    height: 100px;
    padding: 10px;
    margin: 10px auto;

    /* Tipography */
    font: normal 13px "Helvetica Neue", sans-serif;
    line-height: 1.5;
    color: #333;
    text-align: center;

    /* Visual */
    background-color: #F5F5F5;
    border: 1px solid #E5E5E5;
    border-radius: 3px;

    /* Others */
    opacity: 1;
}
```

**[⬆ back to top](#table-of-contents)**

## Class Name

Keep class lowercase and use dashes.

```css
/* Good */
.nav-item { ... }

/* Bad */
.NavItem { ... }
.nav_item { ... }
```

Dashes serve as natural breaks in related class. Prefix class based on the closest parent or base class.

```css
/* Good */
.navbar { ... }
.nav { ... }
.nav-item { ... }
.nav-link { ... }

/* Bad */
.item-nav { ... }
.link-nav { ... }
```

Avoid giving too short names for class and always choose meaningful names that provide the class function.

```css
/* Good */
.btn { ... }
.page-header { ... }
.progress-bar { ... }

/* Bad */
.s { ... }
.ph { ... }
.block { ... }
```

**[⬆ back to top](#table-of-contents)**

## Performance

Never use IDs.

```css
/* Good */
.header { ... }
.section { ... }

/* Bad */
#header { ... }
#section { ... }
```

Do not use selectors standards for not generic rules, always preferably for class.

```css
/* Good */
.form-control { ... }
.header { ... }
.section { ... }

/* Bad */
input[type="text"] { ... }
header
section
```

Avoid nesting elements, the preference is always to use class.

```css
/* Good */
.navbar { ... }
.nav { ... }
.nav-item { ... }
.nav-link { ... }

/* Bad */
.navbar ul { ... }
.navbar ul li { ... }
.navbar ul li a { ... }
```

Nest only when need change the class comportament with interference for other class. Keep the nested on max of three elements.

```css
/* Good */
.modal-footer .btn { ... }
.progress.active .progress-bar { ... }

/* Bad */
.modal-btn { ... }
.progress.active .progress-bar .progress-item span { ... }
```

Always minify the CSS code. Task builders like [Grunt](http://gruntjs.com/) leaves this easier.

```css
<!-- Good -->
.navbar{ ... }.nav{ ... }.nav-item{ ... }.nav-link{ ... }

<!-- Bad -->
.nav-item {
    ...
}
.nav-link {
    ...
}
```

**[⬆ back to top](#table-of-contents)**

## Import

Compared to <link>s, @import is slower, adds extra page requests, and can cause other unforeseen problems. Avoid them and instead opt for an alternate approach:

```html
<!-- Use link elements -->
<link rel="stylesheet" href="core.css">

<!-- Avoid @imports -->
<style>
  @import url("more.css");
</style>
```

- Use multiple <link> elements
- Compile CSS with a preprocessor like Sass or Stylus into a single file
- Concatenate CSS files with features provided in Rails, Jekyll, and other environments

**[⬆ back to top](#table-of-contents)**

## Media Queries

Start the development with generic rules with and add media queries with mobile first.

```css
/* Good */
.navbar {
    margin-bottom: 20px;
}

@media (min-width: 480px) {
    .navbar {
        padding: 10px;
    }
}

@media (min-width: 768px) {
    .navbar {
        position: absolute;
        top: 0;
        left: 0;
    }
}

@media (min-width: 992px) {
    .navbar {
        position: fixed;
    }
}

/* Bad */
.navbar {
    position: fixed;
    top: 0;
    left: 0;
}

@media (max-width: 767px) {
    .navbar {
        position: static;
        padding: 10px;
    }
}

```

Keep the media queries in a separate stylesheet.

```css
@media (min-width: 480px) {
    .navbar { ... }
    .nav { ... }
    .nav-item { ... }
}
```

**[⬆ back to top](#table-of-contents)**

## Prefixed properties

/* Prefixed properties */
.selector {
  -webkit-box-shadow: 0 1px 2px rgba(0,0,0,.15);
          box-shadow: 0 1px 2px rgba(0,0,0,.15);
}

**[⬆ back to top](#table-of-contents)**

## Shorthand notation

Strive to limit use of shorthand declarations to instances where you must explicitly set all the available values. Common overused shorthand properties include:

- padding
- margin
- font
- background
- border
- border-radius

```css
/* Bad */
.element {
    margin: 0 0 10px;
    background: red;
    background: url("image.jpg");
    border-radius: 3px 3px 0 0;
}

/* Good */
.element {
    margin-bottom: 10px;
    background-color: red;
    background-image: url("image.jpg");
    border-top-left-radius: 3px;
    border-top-right-radius: 3px;
}
```

**[⬆ back to top](#table-of-contents)**

## Pre-Processors

I use pre-processors in all projects. Today I use `Sass` on Ruby or PHP projects and `Stylus` on Full Stack JavaScript projects.

Warning with nesting rules of pre-processors. Continue keep without nesting.

```css
/* Good */
.nav-item { ... }

/* Bad */
.navbar {
    .nav {
        .nav-item {
            ...
        }
    }
}
```

Provide semantic names for variables.

```css
/* Good */
@brand-primary: #049cdb;

/* Bad */
@color-blue: #049cdb;
```

**[⬆ back to top](#table-of-contents)**

## Comments

All comments must be made using the syntax of the preprocessor in use.

```css
//
// Section
// --------------------------------------------------

// Sub-section
// --------------------------------------------------

//
// Commentary block
//

// Simple commentary
```
