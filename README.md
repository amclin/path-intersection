# path-intersection

[![Build Status](https://travis-ci.org/bpmn-io/path-intersection.svg?branch=master)](https://travis-ci.org/bpmn-io/path-intersection)

Computes the intersection between two SVG paths.


## Examples

![Intersection examples](./resources/examples.png)

Execute `npm run dev` and navigate to [`http://localhost:9876/debug.html`](http://localhost:9876/debug.html) to see more examples.


## Usage

```javascript
var intersect = require('path-intersection');

var path0 = 'M30,100L270,20';
var path1 = 'M150,150m0,-18a18,18,0,1,1,0,36a18,18,0,1,1,0,-36z';

var intersection = intersect(path0, path1);
// [ { x: ..., y: ..., segment1: ..., segment2: ... }, ... ]
```


## Building the Project

Perform a full build of the library (lint + test) via

```
npm run all
```


## License

Use under the terms of the [MIT license](http://opensource.org/licenses/MIT).