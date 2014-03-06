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
