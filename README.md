# Baseline

Baseline is a simple boilerplate for building new projects on [Skel](http://github.com/n33/skel). Features include:

- Clear and concise HTML5/CSS3 code.
- Fully responsive.
- Extensively organized Sass sources.
- Off-canvas navigation (built with CSS3 and just a tiny bit of vanilla JS).
- Numerous pre-styled elements.
- Font Awesome icons.
- Everything offered by Skel + Skel.scss, including:
	- A powerful, fully responsive CSS grid system.
	- Handy utility classes (like `container`).
	- Breakpoint events (eg. `skel.on("+small", function() { /* do something when the "small" breakpoint becomes active */ });`).

_Note: This version of Baseline is built on [Skel 3](http://github.com/n33/skel) (currently in active development)._


## File Structure

Here's a quick overview of how Baseline's files are organized:

File                        | Description
----------------------------|----------------------------------------------------------
`index.html`                | Main HTML
`assets/`                   | Assets
`  css/`                    | Stylesheets
`    main.css`              | Main stylesheet
`    font-awesome.min.css`  | Font Awesome's stylesheet
`  fonts/*`                 | Font Awesome's webfont files
`  js/`                     | Scripts
`    skel.min.js`           | Skel (JS framework)
`    main.js`               | Main JS (initializes Skel, off-canvas navigation, etc.)
`  sass/`                   | Sass sources
`    main.scss`             | Main Sass stylesheet
`    base/*`                | Base styles
`    components/*`          | Reusable components (box, button, form, etc.)
`    layout/*`              | Primary layout components (header, footer, etc.)
`    libs/`                 | Helper libraries
`      _skel.scss`          | Skel.scss (Sass framework)
`      _vars.scss`          | Variables
`      _functions.scss`     | Functions
`      _mixins.scss`        | Mixins


## Breakpoint Structure

Baseline is set up to use the following breakpoints:

Name*                     | Media Query
--------------------------|-----------------------
`xlarge`                  | `(max-width: 1680px)`
`large`                   | `(max-width: 1280px)`
`medium`                  | `(max-width: 980px)`
`small`                   | `(max-width: 736px)`
`xsmall`                  | `(max-width: 480px)`

If you need to change these, they're explicitly defined in _two_ separate places:

- `assets/js/main.js`

	Enables Skel's breakpoint events and other breakpoint-related functionality.

- `assets/sass/main.scss`

	Enables the use of the Skel.scss's `breakpoint()` mixin and adds responsiveness to its various layout tools (grid system, containers, etc).


## Credits

- Font Awesome (http://fontawesome.io | (c) Dave Gandy | MIT license)
- classList (http://github.com/remy/polyfills | (c) @remy | rem.mit-license.org)
- Skel + Skel.scss (http://skel.io | (c) n33 | MIT license)


## License

Baseline is released under the MIT license.

Copyright (c) n33

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.