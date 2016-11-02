# Tip
A simple jQuery Tip plugin.

## HTML Markup
``` html
&lt;button class="tip" data-position="top-left" data-tip="Tip text here"&gt;Tip shows top left&lt;/button&gt;
```
## Usage
``` js
// use as jquery plugin
$(".tip").tip();

// use as Independent object
new Tip({
    // configration stuff herr
});

// use as CommonJS and CommonJS-like environments
var Tip = require("tip");
```

## Configration
``` js
$(".tip").tip({
    // the target DOM element of ID selector
    target: "#tip",
    // Tip text or the "data-tip" property of the target element
    tip: "Tip is a useful jQuery plugin",
    // tip display position (or "data-position" of the target element, "bottom-center" as default value)
    position: "left",
    // the HTML template of the root DOM element
    TIP_WRAP: '&lt;div class="tip-wrap {position} ' + CLS_HIDE + '" id="tip-{id}"&gt;&lt;/div&gt;',
    // the HTML template of the content DOM element
    TIP_CONTENT: '&lt;div class="tip-content">{content}&lt;/div&gt;'
});
```

## License

Code licensed under <a href="http://opensource.org/licenses/mit-license.html">MIT License</a> · API
Documentation licensed under <a href="http://creativecommons.org/licenses/by/3.0/">CC BY 3.0</a>
