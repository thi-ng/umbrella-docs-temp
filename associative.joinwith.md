<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/associative](./associative.md) &gt; [joinWith](./associative.joinwith.md)

## joinWith variable

Similar to [join](./associative.join.md)<!-- -->, computes the join between two sets of relations, using the given keys in `kmap` only for joining and ignoring others. `kmap` can also be used to translate join keys in `b` where needed. Else, if no renaming is desired, the values in `kmap` should be the same as their respective keys, e.g. `{id: "id"}`<!-- -->. Returns new set of same type as `a`<!-- -->.

<b>Signature:</b>

```typescript
joinWith: <A, B>(a: Set<A>, b: Set<B>, kmap: { [id in keyof A]?: keyof B | undefined; }) => Set<any>
```

## Example


```ts
joinWith(
  new Set([
    {id: 1, name: "foo"},
    {id: 2, name: "bar"},
    {id: 3, name: "baz"}]),
  new Set([
    {type: 1, color: "red"},
    {type: 2, color: "blue"}]),
  {id: "type"}
)
// Set {
//   { type: 1, color: 'red', id: 1, name: 'foo' },
//   { type: 2, color: 'blue', id: 2, name: 'bar' } }

```

