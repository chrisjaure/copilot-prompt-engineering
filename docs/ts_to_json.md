# Create mock data from types

<!--

Copilot Instructions:
- Prompt the user for a typescript type if one was not provided.

-->

## Input

Provide a valid Typescript type. Example:

```ts
type Pet = {
    name: string
    age: number
}
```

## Output

Generate JSON that matches the type. Fill in random information using the type name and properties as hints. Example:

```ts
const myDog: Pet = {
    name: "Fido",
    age: 5
}
```
