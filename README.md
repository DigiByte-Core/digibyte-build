# digibyte-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install digibyte-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var digibyteTasks = require('digibyte-build');

digibyteTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var digibyteTasks = require('digibyte-build');
digibyteTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/digibyte/digibyte.js) on the main bitcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).

Copyright 2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.

