# NodeJS Style Guide

## Table of Contents
- [Syntax](#syntax)
- [Variables](#variables)
- [Arrays and Objects](#arrays-and-objects)
- [Performance](#performance)
- [Comments](#comments)
- [Documentation](#documentation)

## Syntax

Use soft tabs with 4 (four) spaces. You can configure your editor for this.

```html
<!-- Good -->
var foo = require('foo'),
    bar = require('bar');

var baz = function(res, error) {
    ...
    if (error) {
        throw error;
    }
}

<!-- Bad -->
var foo = require('foo'),
  bar = require('bar');

var baz = function(res, error) {
  ...
  if (error) {
    throw error;
  }
}
```

##### Newlines

Use UNIX-style newlines (\n), and a newline character as the last character of a file. Windows-style newlines (\r\n) are forbidden inside any repository.

##### No trailing whitespace

Just like you brush your teeth after every meal, you clean up any trailing whitespace in your JS files before committing. Otherwise the rotten smell of careless neglect will eventually drive away contributors and/or co-workers.

##### Use Semicolons

According to scientific research, the usage of semicolons is a core values of our community. Consider the points of the opposition, but be a traditionalist when it comes to abusing error correction mechanisms for cheap syntactic pleasures.

##### 80 characters per line

Limit your lines to 80 characters. Yes, screens have gotten much bigger over the last few years, but your brain has not. Use the additional room for split screen, your editor supports that, right?

##### Use single quotes

Use single quotes, unless you are writing JSON.

```javascript
// bad
var name = "Vitor Britto";

// good
var name = 'Vitor Britto';

// bad
var fullName = "Vitor " + this.lastName;

// good
var fullName = 'Vitor ' + this.lastName;
```

##### Opening braces go on the same line

Your opening braces go on the same line as the statement.

```javascript
// good
if (true) {
  console.log('winning');
}

// bad
if (true)
{
  console.log('losing');
}
```

Also, notice the use of whitespace before and after the condition statement.


## Variables

Declare one variable for all var statement (or wherever they make sense).

```javascript
// good
var keys = ['foo', 'bar'],
    values = [23, 42],
    object = {},
    key;

while (items.length) {
  key = keys.pop();
  object[key] = values.pop();
}

// bad
var keys   = ['foo', 'bar'];
var values = [23, 42];

var object = {};
while (items.length) {
  var key = keys.pop();
  object[key] = values.pop();
}
```

##### Use lowerCamelCase for variables, properties and function names

Variables, properties and function names should use lowerCamelCase. They should also be descriptive. Single character variables and uncommon abbreviations should generally be avoided.

```javascript
// good
var adminUser = db.query('SELECT * FROM users ...');

// bad
var admin_user = db.query('SELECT * FROM users ...');
```

##### Use PascalCase for Constructors or classes names

```javascript
// good
function BankAccount() {
    ...
}

// bad
function bank_Account() {
    ...
}
```

##### Use UPPERCASE for Constants

Constants should be declared as regular variables or static class properties, using all uppercase letters.

Node.js / V8 actually supports mozilla's const extension, but unfortunately that cannot be applied to class members, nor is it part of any ECMA standard.

```javascript
// good
var SECOND = 1 * 1000;

function File() {
    ...
}

File.FULL_PERMISSIONS = 0777;

// bad
const SECOND = 1 * 1000;

function File() {
    ...
}

File.fullPermissions = 0777;
```

## Arrays and Objects

Use trailing commas and put short declarations on a single line. Only quote keys when your interpreter complains:

```javascript
// good
var a = ['hello', 'world'];
var b = {
    good: 'code',
    'is generally': 'pretty'
};

// bad
var a = [
    'hello', 'world'
];
var b = {"good": 'code'
        , is generally: 'pretty'
        };

```

Do not extend the prototype of native JavaScript objects. Your future self will be forever grateful.

```javascript
// good
var a = [];
if (!a.length) {
    console.log('winning');
}

// bad
Array.prototype.empty = function() {
    return !this.length;
}

var a = [];
if (a.empty()) {
    console.log('losing');
}
```

## Performance

Any non-trivial conditions should be assigned to a descriptively named variable or function:

```javascript
// good
var isValidPassword = password.length >= 4 && /^(?=.*\d).{4,}$/.test(password);

if (isValidPassword) {
    console.log('winning');
}

// bad
if (password.length >= 4 && /^(?=.*\d).{4,}$/.test(password)) {
    console.log('losing');
}
```

Use the triple equality operator as it will work just as expected.

```javascript
// good
var a = 0;
if (a === '') {
    console.log('winning');
}

// bad
var a = 0;
if (a == '') {
    console.log('losing');
}
```

The ternary operator should not be used on a single line. Split it up into multiple lines instead.

```javascript
// good
var foo = (a === b)
    ? 1
    : 2;

// bad
var foo = (a === b) ? 1 : 2;
```

##### Write small functions

Keep your functions short. A good function fits on a slide that the people in the last row of a big room can comfortably read. So don't count on them having perfect vision and limit yourself to ~15 lines of code per function.

##### Return early from functions

To avoid deep nesting of if-statements, always return a function's value as early as possible.

```javascript
// good
function isPercentage(val) {
    if (val < 0) {
        return false;
    }

    if (val > 100) {
        return false;
    }

    return true;
}

// bad
function isPercentage(val) {
    if (val >= 0) {
        if (val < 100) {
            return true;
        } else {
            return false;
        }
    } else {
        return false;
    }
}

// Or for this particular example it may also be fine to shorten things even further:
function isPercentage(val) {
    var isInRange = (val >= 0 && val <= 100);
    return isInRange;
}
```

##### Name your closures

Feel free to give your closures a name. It shows that you care about them, and will produce better stack traces, heap and cpu profiles.

```javascript
// good
req.on('end', function onEnd() {
    console.log('winning');
});

// bad
req.on('end', function() {
    console.log('losing');
});
```

##### No nested closures

Use closures, but don't nest them. Otherwise your code will become a mess.

```javacript
// good
setTimeout(function() {
    client.connect(afterConnect);
}, 1000);

function afterConnect() {
    console.log('winning');
}

// bad
setTimeout(function() {
    client.connect(function() {
        console.log('losing');
    });
}, 1000);
```

## Comments

Use slashes for both single line and multi line comments. Try to write comments that explain higher level mechanisms or clarify difficult segments of your code. Don't use comments to restate trivial things.

```javascript

// good

// 'ID_SOMETHING=VALUE' -> ['ID_SOMETHING=VALUE'', 'SOMETHING', 'VALUE']
var matches = item.match(/ID_([^\n]+)=([^\n]+)/));

// This function has a nasty side effect where a failure to increment a
// redis counter used for statistics will cause an exception. This needs
// to be fixed in a later iteration.
function loadUser(id, cb) {
    // ...
}

var isSessionValid = (session.expires < Date.now());
if (isSessionValid) {
    // ...
}


// bad

// Execute a regex
var matches = item.match(/ID_([^\n]+)=([^\n]+)/));

// Usage: loadUser(5, function() { ... })
function loadUser(id, cb) {
  // ...
}

// Check if the session is valid
var isSessionValid = (session.expires < Date.now());
// If the session is valid
if (isSessionValid) {
  // ...
}
```

## Documentation

> TODO
