# Functions
A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output.

```sh
function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}

let x = myFunction(4, 3);
console.log(x);
```
> output: 12

# Why Functions
You can reuse code: Define the code once, and use it many times. You can use the same code many times with different arguments, to produce different results.

# Examples

```sh
function myFunction() {
  alert("Hello World!");
}```

> output: Notice its output


```sh
function square(number) {
  return number * number;
}

console.log(square(5));
console.log(square(9));
console.log(square(4));
```

> output: 25
> 81
> 16

```sh
const factorial = function fac(n) {
  return n < 2 ? 1 : n * fac(n - 1);
}

console.log(factorial(3));
console.log(factorial(5));
```

> output: 6
> Saab 120

The above example can be rewritten as follows:
```sh
function factorial(n) {
  if (n === 0 || n === 1) {
    return 1;
  } else {
    return n * factorial(n - 1);
  }
}
const c = factorial(3); // c gets the value 6
const d = factorial(4); // d gets the value 24
```

# Nested Functions

```sh
function addSquares(a, b) {
  function square(x) {
    return x * x;
  }
  return square(a) + square(b);
}
const a = addSquares(2, 3); // returns 13
const b = addSquares(3, 4); // returns 25
const c = addSquares(4, 5); // returns 41
```

# Rest Parameters
The rest parameter syntax allows us to represent an indefinite number of arguments as an array.

```sh
function multiply(multiplier, ...theArgs) {
  return theArgs.map((x) => multiplier * x);
}

const arr = multiply(2, 1, 2, 3);
console.log(arr); // [2, 4, 6]
```

# Arrow Function
They are just another way of creating the functions nothing special.

```sh
const a = [
  'Hydrogen',
  'Helium',
  'Lithium',
  'Beryllium'
];

const a2 = a.map(function(s) { return s.length; });

console.log(a2); // logs [8, 6, 7, 9]

const a3 = a.map((s) => s.length);

console.log(a3); // logs [8, 6, 7, 9]

```
