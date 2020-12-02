# JS Fundamentals

- *all of the code below is running in either [strict mode](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode), or in an ES6 module*

## I. Primitive types (aka value) v. Reference Types

- A primitive type (e.g. `Number`, `Boolean`, `null`, `undefined`) has a fixed size in memory. `Number` occupies eight bytes of memory, and a `Boolean` value can be represented with only one bit. We say that they are stored *by value*.
- `Object` and `Array` types do not have a fixed size. Instead, the variable stores a *reference* (e.g. pointer or memory address) to the value. This reference is not the data value itself, but it tells the variable where to look to find the value.
- Strings ARE variable size (like reference types), but because they immutable they behave like value types (see the HW below)


### I-A. *Value* type example

```js
let a = 3.14;    // Declare and initialize a variable
let b = a;       // Copy the variable's value to a new variable
a = 3;           // Modify the value of the original variable
console.log(a);  // Displays 3 as expected
console.log(b);  // Displays 3.14; the copy has not changed
```

### I-B. *Reference* type example

```js
let a = [1,2,3];    // Initialize a variable to refer to an array
let b = a;          // Copy that reference into a new variable
a[0] = 100;          // Modify the array using the original variable's reference
console.log(a);     // Display the changed array [100,2,3] via the original variable
console.log(b);     // Display the changed array [100,2,3] via the new variable
/* Thus `a` and `b` are pointing at the same array! */
```


## XXX. 
