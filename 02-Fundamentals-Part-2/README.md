### Strict mode

```javascript
"use strict";
```

### Functions

```javascript
// function
function logger1() {
  console.log("Me Mohit1");
}

// anyon function
const logger2 = function () {
  console.log("Me Mohit2");
};

// arrow function
const logger3 = () => {
  console.log("Me Mohit3");
};

logger1();
logger2();
logger3();
```

### Functions inside functions

### Reviewing functions

### Arrays

### Array operations

```javascript
friends.push("Miles");
friends.unshift("Gwen");
// push and unshift function return the new length of the array

console.log(friends.indexOf("Miles"));
console.log(friends.includes("Miles"));
```

### Objects

### Dot and bracket notation

```javascript
const mohit = {
  _name: "Mohit",
  _age: "22",
  _job: "student",
};

console.log(mohit._name);
let nameKey = "_name";
console.log(mohit[`${nameKey}`]);

mohit._color = "Blue";
```

### Objects Methods

Function attached to a object
this keyword "current calling object"

### Loops

for loop
while loop
