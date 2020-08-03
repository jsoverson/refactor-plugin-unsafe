## Shift Refactor Plugin: Unsafe methods

This is a plugin for `shift-refactor`. These methods are useful and commonly used but the implementations are not perfect and may transform JavaScript incorrectly.

## Installation

```
$ npm install refactor-plugin-unsafe
```

## Usage

```js
const {refactor} = require('shift-refactor');
const unsafeMethods = require('refactor-plugin-unsafe');

const src = `/* js source */`;

const $script = refactor(src, unsafeMethods);
```

## API

### Methods

- [`.massRename(namePairs)`](#massRenamenamePairs)

#### `.method(namePairs)`

Rename a list of variables.

#### Example

```js
$script.massRename([['fromName', 'toName']]);
```
