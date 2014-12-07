# JavaScript Next snippets

My personal flavor of JavaScript Next snippets for Sublime Text 3.

I was unhappy with the state of existing snippets, so I created my own. Will be adding snippets for newer JavaScript features as I experiment with them.


## Installation

**WARNING:** Only tested on Mac OS X, other paths found from (Sublime Text Unofficial Documentation)[http://docs.sublimetext.info/en/latest/] and may be inaccurate

### Mac OS X
```sh
git clone git://github.com/cesarandreu/sublime-javascript-next-snippets.git ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/javascript-next-snippets
```

### Linux
```sh
git clone git://github.com/cesarandreu/sublime-javascript-next-snippets.git ~/.config/sublime-text-3/Packages/javascript-next-snippets
```

### Windows
```sh
git clone git://github.com/cesarandreu/sublime-javascript-next-snippets.git %APPDATA%\Sublime^ Text^ 3\Packages\javascript-next-snippets
```


## Snippets

### console

#### console.assert

**trigger:** `ca`

```javascript
console.assert(expr, 'msg');
```

#### console.count

**trigger:** `cc`

```javascript
console.count('label');
```

#### console.dir

**trigger:** `cd`

```javascript
console.dir(obj);
```

#### console.error

**trigger:** `ce`

```javascript
console.error(err);
```

#### console.log

**trigger:** `cl`

```javascript
console.log(msg);
```

#### console.trace

**trigger:** `ct`

```javascript
console.trace(err);
```


### functions

#### anonymous function

**trigger:** `afn`

```javascript
function (args) {
  // body
}
```

#### generator function

**trigger:** `gfn`

```javascript
function* name (args) {
  // body
}
```

#### named function

**trigger:** `fn`

```javascript
function name (args) {
  // body
}
```

#### variable function

**trigger:** `vfn`

```javacript
var name = function name (args) {
  // body
};
```

#### immediately-invoked function

**trigger:** `iifn`

```javacript
(function () {
  // body
})();
```


### control flow

#### if

**trigger:** `if`

```javascript
if (condition) {
  // body
}
```

#### if else

**trigger:** `ife`

```javascript
if (condition) {
  // if body
} else {
  // else body
}
```


### iterations

#### for

**trigger:** `for`

```javascript
for (var i = 0; i < arr.length; i++) {
  arr[i]
}
```

#### improved for

**trigger:** `fori`

```javascript
for (var i = 0, len = arr.length; i < len; i++) {
  arr[i]
}
```

#### reverse for

**trigger:** `forr`

```javascript
for (var i = arr.length - 1; i >= 0; i--) {
  arr[i]
}
```

#### for-in

**trigger:** `forin`

```javascript
for (var prop in obj) {
  if (obj.hasOwnProperty(prop)) {
    obj[prop]
  }
}
```


### packages

#### require (CommonJS)

**trigger:** `req`

```javascript
require('package')
```


### testing

#### BDD after each

**trigger:** `ae`

```javascript
afterEach(function () {
  // body
});
```

#### BDD before each

**trigger:** `be`

```javascript
beforeEach(function () {
  // body
});
```

#### BDD describe

**trigger:** `desc`

```javascript
describe('description', function () {
  // body
});
```

#### BDD it (async)

**trigger:** `ita`

```javascript
it('statement', function (done) {
  // body
});
```

#### BDD it (generators)

**trigger:** `itg`

```javascript
it('statement', function* () {
  // body
});
```

#### BDD it (sync)

**trigger:** `its`

```javascript
it('statement', function () {
  // body
});
```


### other

#### setInterval

**trigger:** `si`

```javascript
setInterval(function () {
  // body
}, ms);
```

#### setTimeout

**trigger:** `st`

```javascript
setTimeout(function () {
  // body
}, ms);
```


## Inspiration

To create this I shamelessly ripped and tweaked existing snippets, so thanks to all JavaScript snippets inside Package Control!


## License

MIT
