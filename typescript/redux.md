```js
const loginRequest = {
    type: 'LOGIN_REQUEST',
    payload: {
        name: 'admin',
        password: '123',
    },
};
```

This is what the type signature looks like in TypeScript

```ts
type Action = {
    type: string;
    payload?: any;
    meta?: any;
    error?: boolean;
};
```