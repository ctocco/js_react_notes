# Scope - If and functions

Only functions are block scoped in javascript. Therefore variable declared in if statements are hoisted.

- Using let can solve this issue of hoisting with if statements

```js
// as let is block scoped it is best to declare the variable outside the if statement

let animal;

if (true) {
  animal = "cheetah";
} else {
  animal = "no animal";
}

console.log(animal);
```

Source: https://stackoverflow.com/questions/6964895/javascript-variable-scope-in-the-if-statement
