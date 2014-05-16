# strings-parser-date [![NPM version](https://badge.fury.io/js/strings-parser-date.png)](http://badge.fury.io/js/strings-parser-date)

> Parser for strings to handle date parsing.

## Install
Install with [npm](npmjs.org):

```bash
npm i strings-parser-date --save
``` 

## Usage
Add as a `strings` parser:

```js
var Strings = require('strings');
var date = require('strings-parser-date');

var strings = new Strings();
strings.parser('date', date());

var context = {
  date: '2014-MAY-15'
};
var template = ':YYYY';
var str = strings.template(template, 'date', context);

// expected: '2014'
console.log(str);
```

## Author

**Brian Woodward**

+ [github/doowb](https://github.com/doowb)
+ [twitter/doowb](http://twitter.com/doowb)


## License
Copyright (c) 2014 Brian Woodward, contributors.  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on May 15, 2014._
