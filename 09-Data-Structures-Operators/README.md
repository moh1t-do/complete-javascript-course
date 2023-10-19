### Destructuring

```javascript
// destructuring
const [x, y, z] = arr;

// skipping is also applicable
const [x, , y] = arr;

// applicable for swapping
[a, b] = [b, a];

// nested destructing
const [x, [y, z]] = arr;

// adding default values
const [x = 1, y = 2] = arr;
```

### Spread

unpacking of contents; is on the right side

```javascript
const arr = [1, 2, 3];
const newArray = [...arr, 4];
```

### Rest

Accumulation of contents; is on the left side used with destructuring operator.

```javascript
const [a, ...b] = [1, 2, 3, 3];
```

### Short Circuiting

Usage of &&, ||;

```javascript
console.log(3 && "Miles"); // Miles; End or first false value
console.log(3 || "Miles"); // 3; First true value
```

### Nullish Operator

Works for nullish values rather than false values
null and undefined

### Loops

```javascript
// to get only the current element
for (const item in menu) console.log(item);

// to get index and current element
for (const [idx, ele] in menu.entries()) console.log(`${idx} : ${ele}`);
```

### Enhanced Object Literals

- function outside object.
- binding fucntions.

### Optional Chaining

```javascript
console.log(res.open.mon?.open);
```

### Iterating over Objects

```javascript
// to get keys
for (const day of Object.keys(openingHours)) console.log(day);

// to get keys
for (const day of Object.values(openingHours)) console.log(day);
```

### Set

```javascript
const orderSet = new Set(`an iterable`);
const orderSet = new Set(["Pasta", "Pasta", "Pizza"]);
```

### Map

Maps can have any data type as keys unlike objects which only should be strings.
Object are not iterables hence .entries() is used.

### String
