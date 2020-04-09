<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [DerefedKeys](./api.derefedkeys.md)

## DerefedKeys type

Constructs a type with a set of properties `K` of type `T` and attempts to resolve each given key via [Derefed](./api.derefed.md)<!-- -->.

<b>Signature:</b>

```typescript
export declare type DerefedKeys<T extends IObjectOf<any>, K extends keyof T = keyof T> = {
    [P in K]: Derefed<T[P]>;
};
```

## Example


```ts
interface Foo {
    a: IDeref<string>;
    b: IDeref<number>;
    c: { d: number };
}

type Foo2 = DerefedKeys<Foo>;
// { a: string; b: number; c: { d: number; } }

type Foo3 = DerefedKeys<Foo, "b">;
// { b: number; }

```
