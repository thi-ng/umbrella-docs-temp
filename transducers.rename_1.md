<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [rename](./transducers.rename_1.md)

## rename() function

<b>Signature:</b>

```typescript
export declare function rename<A, B>(kmap: IObjectOf<PropertyKey> | Array<PropertyKey>, rfn: Reducer<B, [PropertyKey, A]>, src: Iterable<A[]>): IterableIterator<B>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  kmap | <code>IObjectOf&lt;PropertyKey&gt; &#124; Array&lt;PropertyKey&gt;</code> |  |
|  rfn | <code>Reducer&lt;B, [PropertyKey, A]&gt;</code> |  |
|  src | <code>Iterable&lt;A[]&gt;</code> |  |

<b>Returns:</b>

`IterableIterator<B>`
