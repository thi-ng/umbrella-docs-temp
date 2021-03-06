<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/system](./system.md) &gt; [SystemSpecs](./system.systemspecs.md)

## SystemSpecs type

Definition object of system component specs, i.e. their factories and component dependencies. The generic type arg `T` is used to infer &amp; validate all specs.

<b>Signature:</b>

```typescript
export declare type SystemSpecs<T extends SystemMap<T>> = Record<Keys<T>, {
    factory: ComponentFactory<T>;
    deps?: Keys<T>[];
}>;
```
