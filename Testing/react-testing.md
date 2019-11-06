# Testing in React

Jest comes with react app

install @testing-library/react react-test-render jest-dom --save-dev

```js
function Button({ label }) {
  return <div data-testid="button">{label}</div>;
}
```

data-\* is an HTML attribute that allows you to store some (https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes)[extra information] that doesn’t have any visual representation. You can use this to test dom element instead of using actual IDs which could change over time.
