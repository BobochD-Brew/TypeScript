Fork of [typescript](https://github.com/microsoft/TypeScript)

### Expose TupleType's members names

```ts
const f = (arg_1: string, arg_2: number) => {};
type params = Parameters<typeof f>; // [string, number]
type names = params["$byName"] // { arg_1: string, arg_2: number }
```
