# parse-key-value
JavaScript parser for key1=value1;"key 2"="value 2"; strings.

## Installation

```sh
npm install --save parse-key-value
```

## Usage

```javascript
const string = "id=myId;description='My test string';weight=0.5;bool=true";

const parse = require('parse-key-value');

// either create a new object:
const object = parse(string);

// or extend an existing one:
const object = {};
parse(string, object);
```

should result in:

```javascript
const object = {
    id: "myId",
    description: "My test string",
    weigth: 0.5,
    bool: true
};
```

## Notes & license
This project is available on [GitHub](https://github.com/StefanHamminga/parse-key-value.js) and [npm](https://www.npmjs.com/package/parse-key-value).

The project is licensed as [MIT](https://opensource.org/licenses/MIT), the license file is included in the project directory.

Copyright 2016 [Stefan Hamminga](mailto:stefan@prjct.net) - [prjct.net](https://prjct.net)
