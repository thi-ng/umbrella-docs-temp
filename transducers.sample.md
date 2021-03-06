<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [sample](./transducers.sample.md)

## sample() function

Transducer which only yields values with given `prob` probability (0.0 .. 1.0 range). Supports custom PRNGs via [IRandom](./random.irandom.md) interface.

<b>Signature:</b>

```typescript
export declare function sample<T>(prob: number): Transducer<T, T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  prob | <code>number</code> |  |

<b>Returns:</b>

`Transducer<T, T>`

## Example


```ts
// 10% probability
[...sample(0.1, range(100))]
// [ 3, 24, 25, 36, 43, 49, 59, 64, 82, 86, 89 ]

```

