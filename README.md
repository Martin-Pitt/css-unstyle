# unstyle.css

Specialised stylesheet for removing user agent styles.

For a demo against the HTML5 Kitchen Sink: http://codepen.io/nexii/pen/WwQXZe?editors=1100

## Install

1. Download [unstyle.css](unstyle.css)
2. Link as first stylesheet:

```html
<link rel="stylesheet" href="css/unstyle.css">
```

## Why?

I believe that by starting from scratch, a blank canvas, we can be free to style the web without the burden of legacy.

As web developers we constantly try to layer our own baseline on the web. Having worked on many lightweight websites and webapps I found however being able to start from ground zero, without useragent styles dictating the baseline, I was able to prototype faster and also build more maintainable websites.


## What makes this different from Reset or Normalize?

Rather than serving a baseline or working around inconsistencies, this stylesheet instead seeks to undo all historical legacy browser styles. Giving you a clean slate, so that for example `<h1>`, `<h2>`, `<h3>`, etc, behave and look like a margin-free `<p>`.

This allows you to build up a website from scratch, creating your own definitions and style guides rather than layering ontop of an existing and vague baseline defined by the accidents of history.


Unlike reset/normalize which seek to remove or stabilise browser inconsistencies/styling, unstyle.css instead:
- fights back against user agent styling opinions
- unstyling elements down to barebones

Thus the goal of unstyle.css is to:
- remove user agent opinion
- give you peace of mind


## Contributing

If you feel something is off, feel free to fire an issue.

Pull Requests are welcome. However if I can't pull it (e.g. doesn't match goals), I encourage you to have your own fork :)


## This sounds great but what are the gotchas?

It is not all-encompassing, I had to skip `input` and other form unstyling as there are harsh browser limitations with CSS on those, which would otherwise make unstyle.css too opinionated by itself.

Thus I leave it up to you to style:
- `<input>`, `<textarea>`, `<select>` and all other form elements


Additionally the intended browser support is:
- Modern browsers (Chrome, Firefox, Safari)
- iOS5+
- IE7+
- Android 4+

Browers outside that may not be fully unstyled.

I (Martin Pitt) have however used it in many real world production projects and it has served me well.


Critical feedback/critique is welcome.
