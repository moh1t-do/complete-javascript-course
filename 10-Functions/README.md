Adding default parameter is applicable.

Objects are passed as reference by default. Primitive data types are passed as value.

### First class and Higher order functions.

This keyword is dynamic.

### Call, Apply and Bind

```javascript
// Call
book.call(eurowing, 23, "Sarha");
const args = [23, "Sarha"];
book.call(eurowing, 23, ...args);

// bind
book.apply(eurowing, args);
```

```javascript
// Bind method : Modern way
const bookEW = book.bind(eurowings);
const bookLX = book.bind(swiss);

bookEW("121", "Steve");
// book for EW specifically
const bookEW23 = book.bind(eurowings, 23);
bookEW23("Jonas");
bookEW23("Martha");

// partial application
const addTac = (rate, value) => value + value * rate;
const addVAT = addTax.bind(null, 0.23);
addVAT(12);
```

### IIFE

```javascript
(function () {
  console.log("ONCE !");
})();
```

### Closures

Make a function remember at birth place.
A function has acess to the variable enviroment of the execution context in which it was created.

```javascript
const secureBooking = function(){
  let passengerCount = 0;

  return function (){
    passengerCount++;
    console.log(`${passengerCount} passenger`);
  }
}

const booker = secureBooking();
booker();
booker();
booker();

// output
1 2 3
```
