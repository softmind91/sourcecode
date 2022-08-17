# Arrays(Data Structure)
An array is a data structure, which can hold more than one value.

```sh
const cars = ["Saab", "Volvo", "BMW"];
```
> output: ["Saab", "Volvo", "BMW"]


## `Accessing Array Elements`

You access an array element by referring to the index number:

```sh
const cars = ["Saab", "Volvo", "BMW"];
let car = cars[0];
console.log(car);
```
> output: Saab
Note: Array indexes start with 0.[0] is the first element.[1] is the second element and so on.


## `Changing an Array Element`
```sh
cars[0] = "Opel";
console.log(cars[0]);
```
> output: Opel


## `Adding Array Elements`

```sh
const fruits = ["Banana", "Orange", "Apple"];
fruits.push("Lemon");
console.log(fruits);
```
> output: ["Banana", "Orange", "Apple", "Lemon"]

## `Converting Arrays to Strings`

```sh
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let fruitString = fruits.toString();
console.log(fruitString);
```
> output: Banana,Orange,Apple,Mango


## `join()`

```sh
const fruits = ["Banana", "Orange", "Apple", "Mango"];
console.log(fruits.join(" * "));
```
> output: Banana * Orange * Apple * Mango

## `pop()`
it is used to delete an element from an array.

```sh
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.pop();
console.log(fruits);
```
> output: ["Banana", "Orange", "Apple"]

## `push()`

```sh
const fruits = ["Banana", "Orange", "Apple", "Mango"];
let length = fruits.push("Kiwi");
console(length);
console.log(fruits);
```
> output: 5 and ["Banana", "Orange", "Apple", "Mango", "Kiwi"]

## `shift()`
The shift() method removes the first array element and "shifts" all other elements to a lower index.

```sh
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.shift();
```
> output: ["Orange", "Apple", "Mango"]

## `unshift()`
The unshift() method adds a new element to an array (at the beginning), and "unshifts" older elements:

```sh
const fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.unshift("Lemon");
```
> output: ["Lemon", "Banana", "Orange", "Apple", "Mango"]

## `length`
The length property returns an integer representing the length of the array.
```sh
const fruits = ["Banana", "Orange", "Apple", "Mango"];
console.log(fruits.length);
```
> output: 4

## `concat() -> Merging Two Arrays`
The length property returns an integer representing the length of the array.
```sh
const myGirls = ["Cecilie", "Lone"];
const myBoys = ["Emil", "Tobias", "Linus"];

const myChildren = myGirls.concat(myBoys);
console.log(myChildren);
```
> output: ["Cecilie", "Lone", "Emil", "Tobias", "Linus"];

## `Merging Three Arrays`

```sh
const arr1 = ["Cecilie", "Lone"];
const arr2 = ["Emil", "Tobias", "Linus"];
const arr3 = ["Robin", "Morgan"];
const myChildren = arr1.concat(arr2, arr3);
console.log(myChildren);
```
> output: ["Cecilie", "Lone", "Emil", "Tobias", "Linus", "Robin", "Morgan"]

## `slice()`

```sh
const fruits = ["Banana", "Orange", "Lemon", "Apple", "Mango"];
const citrus = fruits.slice(3);
```
> output: ["Apple", "Mango"]

