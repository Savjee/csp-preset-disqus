# csp-preset-disqus
Disqus preset for [csp-header](https://github.com/frux/csp/tree/master/packages/csp-header#readme)

![npm](https://img.shields.io/npm/v/csp-preset-disqus)
![npm](https://img.shields.io/npm/dw/csp-preset-disqus)

## Installation
```
npm install --save csp-preset-disqus
```

## Usage
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

## Contribute
Feel free to open issues/pull-requests if a directive is missing.