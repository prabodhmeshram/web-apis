## Console API 

Console API is used to write messages to the console from javascript code. 

### console.assert(expression, data)

This method throws error with the data provided as second argument in case of the expression is falsy.

```
const x = 5;
const y = 3;
const reason = 'x is expected to be less than y';
console.assert(x < y, 'x should be less than y');
```

### console.clear()

Clears the current console