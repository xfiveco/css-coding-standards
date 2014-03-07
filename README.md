CSS Coding Standards
====================

CSS Coding Standards you must conform to when writing CSS in XHTMLized projects.

## Terminology

Concise terminology used in these standards:

```css
selector {
	property: value;
}
```

property: value makes a *declaration*. Selector and declarations makes a *rule*.


## Write valid CSS

All CSS code must be valid CSS 2.1 or CSS3.

When using vendor prefixed properties, you can ignore CSS validation errors it generates.

## Indentation

Do not use indentation for selectors.

```css
/* Correct */
.sec-nav {
}

.sec-nav li {
}

.sec-nav li a {
}

.sec-nav li a:hover {
}

/* Wrong */
.sec-nav {}

	.sec-nav li {
	}
 
		.sec-nav li a {
		}
 
			.sec-nav li a:hover {
			}
```

## Line Endings

Files should be formatted with \n as the line ending (Unix line endings), not \r\n (Windows line endings) or \r (Apple OS's). 

## Encoding of CSS files

Encoding of CSS files should be set to UTF-8.

## Naming Conventions

Always use hyphens in class names. Do not use underscores or CamelCase notation.

```css
/* Correct */
.sec-nav

/* Wrong */
.sec_nav
.SecNav
```

## URLs

URLs are written without optional single quote (') or double quote ("):

```css
url(../images/logo.png)
```

## Values
Use pixels to define font sizes:

```css
font-size: 14px;
```

Always define generic font families like sans-serif or serif.

```css
/* Correct */
font-family: "ff-din-web-1", Arial, Helvetica, sans-serif;

/* Wrong */
font-family: "ff-din-web-1";
```

Shorten hexidecimal color values to 3 digits when possible:

```css
background: #fff;
```

Do not use unit with 0.

```css
/* Correct */
.nav a {
	padding: 5px 0 5px 2px;
}

/* Wrong */
.nav a {
	padding: 5px 0px 5px 2px;
}
```

Do not use default values if they are not necessary to override inherited values.
```css
/* Correct */
.nav a {
    background: url(../images/nav.png) no-repeat;
}

/* Wrong */
.nav a {
	background: transparent url(../images/nav.png) no-repeat top left;
}
```
