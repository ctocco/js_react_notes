# When to use React.memo()

1. Pure function component 
- given same props will always render the same output
2. Renders Often
3. Re-renders with the same props
4. Medium to big size 
- should contain a decent amount of UI elements to reason props equality check

-if you have a class use PureComponent which is the memo equivalent. 
