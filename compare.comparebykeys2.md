<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/compare](./compare.md) &gt; [compareByKeys2](./compare.comparebykeys2.md)

## compareByKeys2() function

HOF comparator. Returns new comparator to sort objects by given keys `a` (major), `b` (minor) and with optional comparators (default for each: [compare](./compare.compare.md)<!-- -->).

<b>Signature:</b>

```typescript
export declare function compareByKeys2<T, A extends Keys<T>, B extends Keys<T>>(major: A, minor: B, cmpA?: Comparator<Val1<T, A>>, cmpB?: Comparator<Val1<T, B>>): Comparator<T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  major | <code>A</code> |  |
|  minor | <code>B</code> |  |
|  cmpA | <code>Comparator&lt;Val1&lt;T, A&gt;&gt;</code> |  |
|  cmpB | <code>Comparator&lt;Val1&lt;T, B&gt;&gt;</code> |  |

<b>Returns:</b>

`Comparator<T>`

