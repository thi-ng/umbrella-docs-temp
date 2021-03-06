<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/memoize](./memoize.md) &gt; [memoizeJ](./memoize.memoizej.md)

## memoizeJ() function

Function memoization for arbitrary argument counts. Returns augmented function, which uses `JSON.stringify()` to obtain (and store) memoized result for given args. Supports generics for up to 4 args (otherwise untyped).

\*\*Important:\*\* If the given args cannot be stringified, the user function will ALWAYS be called (without caching result).

<b>Signature:</b>

```typescript
export declare function memoizeJ<A, B>(fn: Fn<A, B>, cache?: IObjectOf<B>): Fn<A, B>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  fn | <code>Fn&lt;A, B&gt;</code> |  |
|  cache | <code>IObjectOf&lt;B&gt;</code> |  |

<b>Returns:</b>

`Fn<A, B>`

