# Loops
Loops are handy, if you want to run the same code over and over again, each time with a different value.

```sh
const cars = ["Saab", "Volvo", "BMW", "Toyota", "Audi", "Suzuki", "Kia"];
let text = "";
text += cars[0] + "<br>";
text += cars[1] + "<br>";
text += cars[2] + "<br>";
text += cars[3] + "<br>";
text += cars[4] + "<br>";
text += cars[5] + "<br>";

console.log(text);
```
> output: <br />
> Saab <br />
> Volvo <br />
> BMW <br />
> Toyota <br />
> Audi <br />
> Suzuki <br />
> Kia <br />

The above code can be written as follows using a for loop:

```sh
const cars = ["Saab", "Volvo", "BMW"];
let text = "";
for (let i = 0; i < cars.length; i++) {
  text += cars[i] + "<br>";
}
console.log(text);
```

> output: <br />
> Saab <br />
> Volvo <br />
> BMW <br />
> Toyota <br />
> Audi <br />
> Suzuki <br />
> Kia

# while
The above code can be written as follows using a while loop:

```sh
const cars = ["Saab", "Volvo", "BMW"];
let text = "";
let i = 0;
while (i < cars.length) {
  text += cars[i] + "<br>";
  i++;
}
console.log(text);
```

> output: <br />
> Saab <br />
> Volvo <br />
> BMW <br />
> Toyota <br />
> Audi <br />
> Suzuki <br />
> Kia

# Do-While

The above code can be written as follows using a do-while loop:

```sh
const cars = ["Saab", "Volvo", "BMW"];
let text = "";
let i = 0;
do {
  text += cars[i] + "<br>";
  i++;
} while(i < cars.length);
console.log(text);
```

> output: <br />
> Saab <br />
> Volvo <br />
> BMW <br />
> Toyota <br />
> Audi <br />
> Suzuki <br />
> Kia

# break
The *break* statement can also be used to jump out of a loop:

```sh
for (let i = 0; i < 10; i++) {
  if (i === 3) { break; }
  text += "The number is " + i + "<br>";
}
```

# continue
The continue statement can only be used to skip one loop iteration.

```sh
for (let i = 0; i < 10; i++) {
  if (i === 3) { continue; }
  text += "The number is " + i + "<br>";
}
```
