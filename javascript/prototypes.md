# Prototypes

```js
function Rectangle() {
  this.x = 4;
  this.y = 6;
}

Rectangle.prototype.area = function() {
  return this.x * this.y;
};

Rectangle.prototype.otherShape = "Square";

let r = new Rectangle();
let r2 = new Rectangle();

console.log(r.area());
console.log(r.square);
```

Above you can see that by creating a prototype we can have the **this** refer to the object that we created. The this LIVES within this object.

We can then add functions and properties to the prototype that can then be shared among all further instatiations of the Rectangle constructor function.

```
__proto__
```

Is actually referring to Object.prototype and is where you will see the methods and properties that you add to the prototype
