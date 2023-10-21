# Arrays

A linear data structure.

### Methods

```javascript
console.log(arr.slice(3)); // no mutation of the array

// forEach pass three parmeter ie element, index and array
arr.forEach(ele => {
  console.log(ele);
});

// reduce
const total = arr.reduce((acc, curval) => acc + curval, 0);

// filter
arr.filter(ele => ele > 0);

// chaining of methods is applicable

// flat & flatMap
const arr = [
  [1, 2, 3],
  [5, 6],
];
console.log(arr.flat(deepth));

// fill
```
