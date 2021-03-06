<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/associative](./associative.md) &gt; [invertMap](./associative.invertmap.md)

## invertMap variable

Returns a new map in which the original values are used as keys and original keys as values. If `dest` is given, writes results in that map instead. Depending on the value type of `src` and/or if the inverted map should use custom key equality semantics as provided by the Map types in this package, you MUST provide a `dest` map, since the default `dest` will only be a standard ES6 Map.

<b>Signature:</b>

```typescript
invertMap: <K, V>(src: Map<K, V>, dest?: Map<V, K> | undefined) => Map<V, K>
```

## Example


```ts
invertMap(new Map(), new Map([["a", 1], ["b", 2]]));
// Map { 1 => 'a', 2 => 'b' }

```

