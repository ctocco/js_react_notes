# FCC Exercises

Check if the value exists in array of objects and also if they are not false

```js
function truthCheck(collection, pre) {
  let isTrue = true;
  collection.map(value => {
    if (!Object.keys(value).includes(pre)) {
      isTrue = false;
    }
    if (!value[pre]) {
      isTrue = false;
    }
  });
  return isTrue;
}

console.log(
  truthCheck(
    [
      { user: "Tinky-Winky", sex: "male" },
      { user: "Dipsy", sex: "male" },
      { user: "Laa-Laa", sex: "female" },
      { user: "Po", sex: "female" }
    ],
    "sex"
  )
);
```

based of the article about Guard Clauses and using less else statements to simplify the look of the code

An example then. Traditionally, you might stop certain code running like this.

```js
const assertString = str => {
  if (typeof str === "string") {
    return true;
  } else {
    return false;
  }
};
```

Using a guard clause, you would write the above like so.

```js
const assertString = str => {
  if (typeof str !== "string") {
    return false;
  }
  return true;
};
```

I’ve adopted this style of exiting everywhere applicable and really like it. I’d encourage you to give it a whirl.
