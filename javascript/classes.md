# Classes in JS

Classes in JS are syntatical sugar and try to imitate what classes are like in other programming languages.

- Classes in JS mimic Object Oriented Programming
- We are aiming for **encapsulation**

## A Class

- is like a template or blueprint
- everything is encapsulated in a class
- has a new keyword -> which means to create an object
- captures data and functionality into an object

```js

Class Exercise {
    constructor(exercise, duration) {
        this.exercise = exercise
        this.duration = duration
    }
}


let exerciseRoutine = new Exercise(yoga, 30)
```
