# ES6
Javascript ES6

1. Perkenalan ES6
V5 = Current Browser supported
Babel = Convert ES6 to ES5

2. const dan let
const => untuk variable yang tidak boleh barubah nilainya
let => untuk variable yang nilainya dapat berubah

3. const and let scope
var bersifat local apabila dalam function tetapi tidak dalam method
let bersifat local dalam function maupun method
```
var name = 'test';
function username() {
var name = 'nontest';
console.log(name);
}

username();
console.log(name);
```
```
var value = 10;
var winner = true;
if (value == 10) {
  var winner = false; // winner = false;
  console.log(winner);
}
console.log(winner);
```

```
const value = 10;
let winner = true;
if (value == 10) {
  let winner = false; // winner = false; => akan mengoverwrite nilai global
  console.log(winner)
}
console.log(winner)
```

```
let winner = 10;
let winner = 40;
Error : Variable already define
```
4. const and let real live example