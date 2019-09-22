# Is Unique

Create a function that checks if all characters in a string are unique.
For `'abcde'`, the return value should be `true`, for `'abccde'` - false.

```js
function makeObject(uniqueArray) {
  let splitArray = uniqueArray.split("");
  let checkUniqueValues = {};
  let isUnique = true;

  for (let i = 0; i < splitArray.length; i++) {
    if (!checkUniqueValues.hasOwnProperty(splitArray[i])) {
      checkUniqueValues[splitArray[i]] = 0;
    }
    checkUniqueValues[splitArray[i]]++;
  }
  Object.values(checkUniqueValues).forEach(e =>
    e > 1 ? (isUnique = false) : null
  );
  return isUnique;
}

console.log(makeObject("abccdee"));
```

Here there is an interesting way to fill an object with values
