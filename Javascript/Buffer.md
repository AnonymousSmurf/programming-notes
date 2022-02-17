# Buffer
The `Buffer` class in Node.js is designed to handle raw binary data. Each buffer corresponds to some raw memory allocated outside V8. Buffers act somewhat like arrays of integers, but aren't resizable and have a whole bunch of methods specifically for binary data. The integers in a buffer each represent a byte and so are limited to values from 0 to 255 inclusive. When using `console.log()` to print the `Buffer` instance, you'll get a chain of values in hexadecimal values.


### Example:
This buffer is initialized and contains 8 bytes of zero.

```js
const buffer = Buffer.alloc(8);
// This will print out 8 bytes of zero:
// <Buffer 00 00 00 00 00 00 00 00>
```

This initializes the buffer to the contents of this array. Keep in mind that the contents of the array are integers representing bytes.

```js
const buffer = Buffer.from([8, 6, 7, 5, 3, 0, 9]);
// This will print out 8 bytes of certain values:
// <Buffer 08 06 07 05 03 00 09>
```

This initializes the buffer to a binary encoding of the first string as specified by the second argument (in this case, `'utf-8'`). `'utf-8'` is by far the most common encoding used with Node.js, but `Buffer` also supports others.

```js
const buffer = Buffer.from("I'm a string!", 'utf-8');
// This will print out a chain of values in utf-8:
// <Buffer 49 27 6d 20 61 20 73 74 72 69 6e 67 21>
```

#JAVASCRIPT 