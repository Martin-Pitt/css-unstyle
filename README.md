# unstyle.css

Specialised stylesheet for removing user agent styles.


## Install

Download [unstyle.css](unstyle.css)
Link as first stylesheet in your html:
```html
<link rel="stylesheet" href="css/unstyle.css">
```


## Why?

I believe that by starting from scratch, a blank canvas, we can be free to style the web without the burden of legacy.


## What makes this different from Reset or Normalize?

Rather than serving a baseline or working around inconsistencies, this stylesheet instead seeks to undo all historical legacy browser styles. Instead giving you a clean slate, for example `<h1>`, `<h2>`, `<h3>`, etc, behave and look like a margin-free `<p>`.

This allows you to build up a website from scratch, creating your own definitions and style guides rather than layering ontop of an existing baseline.


Unlike reset/normalize which seek to remove or stabilise browser inconsistencies/styling, unstyle.css instead:
- fights back against user agent styling opinions
- unstyling elements down to barebones

Thus the goal of unstyle.css:
- remove user agent opinion
- give you peace of mind

## This sounds great but what are the gotchas?

It is not all-encompassing, I had to skip `input` unstyling as there are harsh browser limitations with CSS on those, which would otherwise make unstyle.css too opinionated by itself.

Thus I leave it up to you to style:
- `<input>`, `<textarea>`, `<select>` and all other form elements


Additionally the intended browser support is:
- Modern browsers (Chrome, Firefox, Safari)
- iOS5+
- IE7+
- Android 4+

Browers outside that may not be fully unstyled.

I have however used it in many real world production projects and it has served me well.


Critical feedback/critique is welcome.
