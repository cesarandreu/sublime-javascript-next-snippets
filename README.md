# JavaScript Next snippets

My personal flavor of JavaScript Next snippets for Sublime Text 3.

I was unhappy with the state of existing snippets, so I created my own. Will be adding snippets for newer JavaScript features as I experiment with them.


## Installation

**WARNING:** Only tested on Mac OS X, other paths found from [Sublime Text Unofficial Documentation](http://docs.sublimetext.info/en/latest/) and may be inaccurate

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

trigger: `ca`

```javascript
console.assert(expr, 'msg')
```

#### console.count

trigger: `cc`

```javascript
console.count('label')
```

#### console.dir

trigger: `cd`

```javascript
console.dir(obj)
```

#### console.error

trigger: `ce`

```javascript
console.error(err)
```

#### console.log

trigger: `cl`

```javascript
console.log(msg)
```

#### console.trace

trigger: `ct`

```javascript
console.trace(err)
```


### functions

#### async function

trigger: `afn`

```javascript
async function name (args) {
  // body
}
```

#### generator function

trigger: `gfn`

```javascript
function * name (args) {
  // body
}
```

#### named function

trigger: `fn`

```javascript
function name (args) {
  // body
}
```


### control flow

#### if

trigger: `if`

```javascript
if (condition) {
  // body
}
```

#### if else

trigger: `ife`

```javascript
if (condition) {
  // if body
} else {
  // else body
}
```


### iterations

#### for

trigger: `for`

```javascript
for (var i = 0; i < arr.length; i++) {
  arr[i]
}
```

#### improved for

trigger: `fori`

```javascript
for (var i = 0, len = arr.length; i < len; i++) {
  arr[i]
}
```

#### reverse for

trigger: `forr`

```javascript
for (var i = arr.length - 1; i >= 0; i--) {
  arr[i]
}
```

#### for-in

trigger: `forin`

```javascript
for (var prop in obj) {
  if (obj.hasOwnProperty(prop)) {
    obj[prop]
  }
}
```


### packages

#### require (CommonJS)

trigger: `req`

```javascript
require('package')
```


### testing

#### BDD after each

trigger: `afterEach`

```javascript
afterEach(() => {
  // body
})
```

#### BDD before each

trigger: `beforeEach`

```javascript
beforeEach(() => {
  // body
})
```

#### BDD describe

trigger: `desc`

```javascript
describe('description', () => {
  // body
})
```

#### BDD it

trigger: `its`

```javascript
it('statement', () => {
  // body
})
```


### other

#### setInterval

trigger: `si`

```javascript
setInterval(() => {
  // body
}, ms)
```

#### setTimeout

trigger: `st`

```javascript
setTimeout(() => {
  // body
}, ms)
```


## Inspiration

To create this I shamelessly ripped and tweaked existing snippets, so thanks to all JavaScript snippets inside Package Control!
