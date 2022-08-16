# Control Statement

## `if`

'if' is a control statement that results either True or False not both.The enclosing action is executed only in `True` case e.g.

```sh
let n = 100;
if(n < 100)
    console.log('n is less than 100');
```
> No output: :(   (as `n` is not less than 100)


```sh
let n = 98;
if(n < 100)
    console.log('n is less than 100');
```
> output: n is less than 100


## `if-else`

'if' is a control statement that results either True or False not both.It may result in the execution of either if block or an else block based on `True` and `False` respectively e.g.

```sh
let n = 100;
if(n < 100)
    console.log('n is less than 100');
else
    console.log('n is greater or equal to 100');
```
> output: n is greater or equal to 100


```sh
let n = 98;
if(n < 100)
    console.log('n is less than 100');
else
    console.log('n is greater or equal to 100');
```
> output: n is less than 100


## `nested if`

```sh
let marks = 80;
if(marks > 50)
    if(marks > 80)
        console.log('Pass: A+ Grade')
    else
        console.log('Pass: C Grade');
else
    console.log('Failed! because marks are less than 50');
```
> output: Pass: C Grade
Note: you can try this code with different values of marks like 90, 40


## `Logic Gates`

```sh
let marks = 85;
if(marks > 50 && marks > 80)
    console.log('Pass: A+ Grade')
else
    console.log('Pass: C Grade');

```
> output: Pass: A+ Grade
Note: you can try this code with different values of marks like 40




```sh
let degree = 'matric';
if(degree === 'matric || degree === 'o-level')
    console.log('Admitted')
else
    console.log('Not Admitted');

```
> output: Admitted
Note: you can try this code with different values of degree like `o-level` and `a-level`
