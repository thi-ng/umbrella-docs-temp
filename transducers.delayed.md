<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/transducers](./transducers.md) &gt; [delayed](./transducers.delayed.md)

## delayed variable

Yields transducer which wraps incoming values in promises, which each resolve after specified delay time (in ms).

\*\*Only to be used in async contexts and NOT with `transduce` directly.\*\*

<b>Signature:</b>

```typescript
delayed: <T>(t: number) => Transducer<T, Promise<T>>
```