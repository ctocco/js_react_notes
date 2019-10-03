A generator is a function that can start midway then continue from where it stopped.

It appears as a function but it acts like an iterator.
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Iterators_and_Generators this let's use read more about what an iterator is.
https://codeburst.io/a-simple-guide-to-es6-iterators-in-javascript-with-examples-189d052c3d8e here is a more simple explanation of what they are

In JavaScript, a generator is a function which returns an object on which you can call next(). Every invocation of next() will return an object of shape —

```js
{
  value: Any,
  done: true|false
}
```

The value property will contain the value. The done property is either true or false. When the done becomes true, the generator stops and won’t generate any more values.
