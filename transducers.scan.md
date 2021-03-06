<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [scan](./transducers.scan.md)

## scan() function

Transducer which performs "scan" operation via given reducer.

<b>Signature:</b>

```typescript
export declare function scan<A, B>(rfn: Reducer<B, A>, init?: B): Transducer<A, B>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  rfn | <code>Reducer&lt;B, A&gt;</code> | reducer used as scan operator |
|  init | <code>B</code> |  |

<b>Returns:</b>

`Transducer<A, B>`

## Remarks

[https://en.wikipedia.org/wiki/Prefix\_sum\#Scan\_higher\_order\_function](https://en.wikipedia.org/wiki/Prefix_sum#Scan_higher_order_function)

## Example


```ts
[...iterator(scan(add()), range(10))]
// [ 0, 1, 3, 6, 10, 15, 21, 28, 36, 45 ]

[...scan(add(), null, range(10))]
// [ 0, 1, 3, 6, 10, 15, 21, 28, 36, 45 ]

```

