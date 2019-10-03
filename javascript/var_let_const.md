# Var, Let and Const

1. **var is hoisted**

2. **let and const are not hoisted!**

```js
silver = 20;
console.log(silver);
var silver; // this gets hoisted and is globally scoped

let copper; // let is block scoped so has to come 1st
copper = 20;
console.log(copper);
```

### Let and loops

Loops, while loops or inside the scope of if conditions let is unique to that block while var can be accessed outside of this scope

### const

Literally is a constant which value does not change and is also **block scoped**

```js
const gold = 30;
console.log(gold); // works

const gold;
gold = 30;
console.log(gold); // ERR gold needs to be assigned a value

const gold = 40 // error

// what if it is an object...

const gold = {
  value: 50
}

gold.value = 60 //NO ERR as you are changing the property of gold
```

### Functions

let and var variables work the same way when used in a function block. They are both scoped to the function. In for loops you have to use let.

```js
console.log(varVariable, letVariable); // both not defined as var & let are scoped within function

function sampleFunction() {
  let letVariable = "let";
  var varVariable = "var";

  console.log(letVariable);
  console.log(varVariable);
}

sampleFunction();
```

In if statements or anything that is within a {} the let constant will now be scoped var will not be and will always in those cases be a global variable.
