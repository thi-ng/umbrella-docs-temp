<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [Comparator](./api.comparator.md)

## Comparator type

Generic 2-element comparator function type alias.

<b>Signature:</b>

```typescript
export declare type Comparator<T> = Fn2<T, T, number>;
```

## Remarks

Must follow this contract and return:

- negative if `a < b` - zero if `a == b` - positive if `a > b`

