# copilot-prompt-engineering
Examples of prompt engineering with Copilot

## Prompts

### ts_to_json

#### Prompt

> Follow #file:ts_to_json.md

#### Response

> Sure, let's follow the instructions from the provided documentation. If you have a specific TypeScript type you would like to use, please provide it.

#### Prompt

```ts
type Person = {
    age: number
    occupation: string
}
```

#### Response

> Great! Based on the provided TypeScript type, here is the generated JSON that matches the type:

```ts
const examplePerson: Person = {
    age: 30,
    occupation: "Engineer"
}
```