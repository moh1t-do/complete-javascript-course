# Asynchronous

Async is non-blocking.

### Promise

- An object that is used as a placeholder for the future result of an async operation.
- Work with async operations.

```javascript
const result = fetch("url")
  .then(res => res.json())
  .catch(err => console.log(err))
  .finally(() => console.log("YES"));
console.log(result);

// to read the date we use the json method which is async
// catch to handle errors
// finally that always need to happen eg. hide loader
```

### Chaining Promises

### Throwing Errors

```javascript
throw new Error("message");

// explicitly throwing an error
// will propagate to catch method
```

### Creating Promises

```javascript
const lotteryPromise = new Promise((resolve, reject) => {
  setTimeout(() => {
    if (Math.random() >= 0.5) resolve("You win");
    else reject(new Error("BOO"));
  }, 2000);
});

lotteryPromise.then(res => console.log(res)).catch(err => console.log(err));
```

### Async Function

```javascript
const whereAmI = async () => {
  const res = await fetch("url");
};

// use try catch to handle errors in async await
```
