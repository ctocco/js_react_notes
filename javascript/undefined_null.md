```js
let x = undefined;
console.log(typeof x); // undefined
console.log(x == false);

let y = null;
console.log(typeof y); // object

function checkValue(value) {
  console.log(!!value);
}

checkValue(); // false
checkValue(null); // false
checkValue(undefined); // false
checkValue(false); // false
checkValue(""); // false

checkValue(true); // true
checkValue({}); // true
checkValue("any string"); // true
```

Quick overview

- typeof null gives you an object not null
