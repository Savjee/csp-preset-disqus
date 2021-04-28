# csp-preset-disqus
Disqus preset for [csp-header](https://github.com/frux/csp/tree/master/packages/csp-header#readme)

Installation:
```
npm install --save csp-preset-disqus
```

Usage:
```js
const { getCSP } = require('csp-header');

const my_csp_policy = getCSP({
    directives: {
        // ...
        "script-src": [
            // ...
            "your-disqus-subdomain-name.disqus.com",
        ],
    },
    presets: [
        // Add the Disqus preset
        require("csp-preset-disqus"),
    ]
});
```

Don't forgot the add your Disqus subdomain to the `script-src` directive.