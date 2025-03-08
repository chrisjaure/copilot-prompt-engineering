# copilot-prompt-engineering

This repo contains documents that Copilot can follow to perform tasks.

For other examples, see https://docs.github.com/en/copilot/copilot-chat-cookbook.

## Prompts

### Generate sample JSON from a Typescript type

This document contains a hidden instruction for Copilot to prompt for more information if the user doesn't provide a type in the initial request.

#### Prompt

> Follow [#file:ts_to_json.md](/docs/ts_to_json.md)

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
