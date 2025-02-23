Fork of [typescript](https://github.com/microsoft/TypeScript)

### Expose TupleType's members names

```ts
const f = (arg_1: string, arg_2: number) => {};
type params = Parameters<typeof f>; // [string, number]
type names = params["$byName"] // { arg_1: string, arg_2: number }
```

### Dynamic JSX Elements result type

```ts
export declare namespace JSX {
    export type ElementOf<T> = T;
}
const a = <div /> // a: "div"
const a = <Component /> // a: typeof Component
```
