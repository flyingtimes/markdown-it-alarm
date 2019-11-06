# markdown-it-mark


> `<alarm>` tag plugin for [markdown-it](https://github.com/markdown-it/markdown-it) markdown parser.

__v3.+ requires `markdown-it` v10.+, see changelog.__

`^^marked^^` => `<alarm>marked</alarm>`

Markup uses the same conditions as CommonMark [emphasis](http://spec.commonmark.org/0.15/#emphasis-and-strong-emphasis).


## Install

node.js, browser:

```bash
npm install markdown-it-alarm --save
```

## Use

```js
var md = require('markdown-it')()
            .use(require('markdown-it-alarm'));

md.render('^^marked^^') // => '<p><alarm>marked</alarm></p>'
```

_Differences in browser._ If you load script directly into the page, without
package system, module will add itself globally as `window.markdownitMark`.


## License

[MIT]

