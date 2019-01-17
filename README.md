# Github Wrapper 

[![Build Status](https://travis-ci.org/davidalves1/github-wrapper.svg?branch=master)](https://travis-ci.org/davidalves1/github-wrapper)
[![Coverage Status](https://coveralls.io/repos/github/davidalves1/github-wrapper/badge.svg?branch=master)](https://coveralls.io/github/davidalves1/github-wrapper?branch=master)

A wrapper to work with the [Github Web API](https://developer.github.com/v3/).

## Dependencies

This library depends on [fetch](https://fetch.spec.whatwg.org/) to make requests to the Github Web API. For environments that don't support fetch, you'll need to provide a [polyfill](https://github.com/github/fetch) to browser or [polyfill](https://github.com/bitinn/node-fetch) to Node.

## Installation

```sh
$ npm install github-wrapper --save
```

## How to use

### ES6

```js
// to import a specific method
import { method } from 'github-wrapper';

// to import everything
import * as githubWrapper from 'github-wrapper';
```

### CommonJS

```js
var githubWrapper = require('github-wrapper');
```

### UMD in Browser

```html
<!-- to import non-minified version -->
<script src="github-wrapper.umd.js"></script>

<!-- to import minified version -->
<script src="github-wrapper.umd.min.js"></script>
```

After that the library will be available to the Global as `githubWrapper`. Follow an example:

```js
const user = githubWrapper.getUser('your-user');
```

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors
|  [David Alves](https://github.com/davidalves1/)   |

See also the list of [contributors](https://github.com/davidalves1/js-tdd-course/tree/master/github-wrapper) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
