# Console API 

Console API is used to write messages to the console from javascript code. 

## console.assert(expression, data)

This method throws error with the data provided as second argument in case of the expression is falsy.

```
const x = 5;
const y = 3;
const reason = 'x is expected to be less than y';
console.assert(x < y, 'x should be less than y');

// Assertion failed: x should be less than y
```

## console.clear()

Clears the current console

```
console.clear();
```

## console.count('label')

It prints the number of times a count with particular label has been invoked.
If no label provided, `default` is assigned as label name.

```
console.count('batman');
console.count('batman');
console.count('superman');
console.count('batman');
console.count();

// batman: 1
// batman: 2
// superman: 1
// batman: 3
// default: 1

```

## console.countReset('label')

It basically resets the count set by console.count() method for the lable provided

```
console.count('batman');
console.count('batman');
console.countReset('batman');
console.count('batman');

// batman: 1
// batman: 2
// undefined
// batman: 1

```

## console.debug(data)

Prints log as debug level

```
console.debug('Print me to debug')
// Print me to debug
```

## console.dir(data)

Prints the Json representation of object passed.

```
console.dir({key : "value"})

// { key: "value" }
```

## console.dirxml(node)

Prints an XML representation of the descendants of node

```
console.dirxml(document);

// #document
//  <html lang="en">
//   <head>...</head>
//   <body>...</body>
//  </html>
```

## console.error

Prints log as error level

```
console.error('Print me to error')
// Print me to error
```