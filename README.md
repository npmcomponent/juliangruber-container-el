*This repository is a mirror of the [component](http://component.io) module [juliangruber/container-el](http://github.com/juliangruber/container-el). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/juliangruber-container-el`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# container-el

Use this singleton container element before the DOM is ready.

When the page is loaded, the container will be appended to `<body>`.

## Usage

```js
var container = require('container-el');

var el = document.createElement('div');
el.className = 'has-class';

container.appendChild(el);
```

When the dom is ready, you'll have this:

```html
<!-- ... -->
<body>
  <div id="container">
    <div class="has-class"></div>
  </div>
</body>
<!-- ... -->
```

## Installation

With [npm](https://npmjs.org) do:

```bash
npm install container-el
```

Then bundle for the browser with
[browserify](https://github.com/substack/node-browserify).

With [component](https://github.com/component/component) do:

```bash
component install juliangruber/container-el
```

## License

(MIT)

Copyright (c) 2013 Julian Gruber &lt;julian@juliangruber.com&gt;

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
