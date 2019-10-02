# Unions

Unions fix the problem of the "any" type and gives errors if a certain type outside the desired types. 

for example

```ts
const myFunc (firstValue: string, secondValue: any) {
    if (typeof secondValue = "string") {
        return firstValue + secondValue
    }
    if (typeof secondValue = "number") {
        return secondValue + firstValue
    }
}

myFunc("hello", true) // passes at compile time, fails at runtime.

```

instead now you can use union types

```ts
const myFunc (firstValue: string, secondValue: string | number) {...

}

```