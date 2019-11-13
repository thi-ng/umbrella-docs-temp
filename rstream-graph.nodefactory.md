<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream-graph](./rstream-graph.md) &gt; [NodeFactory](./rstream-graph.nodefactory.md)

## NodeFactory type

A function which constructs and returns an `ISubscribable` using given object of inputs and node ID. See `node()` and `node1()`<!-- -->.

<b>Signature:</b>

```typescript
export declare type NodeFactory<T> = (src: NodeInputs, id: string) => ISubscribable<T>;
```