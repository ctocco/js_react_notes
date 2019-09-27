# what is this?

```js
function Person(age) {
     this.age = age;
     this.growOld = function() {
         this.age++;
     }
 }
 var person = new Person(1);
 setTimeout(person.growOld,1000);
 setTimeout(function() { console.log(person.age); },2000);
 // will return 1 as function points to window object
```


```js
function Person(age) {
    this.age = age;
    this.growOld = () => {
        this.age++;
    }
}
var person = new Person(1);
setTimeout(person.growOld,1000);

setTimeout(function() { console.log(person.age); },2000); // 2 as this refers to lexical context
```