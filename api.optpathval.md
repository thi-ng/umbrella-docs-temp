<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/api](./api.md) &gt; [OptPathVal](./api.optpathval.md)

## OptPathVal type

Similar to [PathVal](./api.pathval.md)<!-- -->, but also takes into account if given path contains any intermediate properties declared as optional in type `T`<!-- -->. If that's the case, returns union of `undefined` and inferred value for path, else just the latter.

Context &amp; reference: https://stackoverflow.com/q/60869412/294515

<b>Signature:</b>

```typescript
export declare type OptPathVal<T, P extends unknown[]> = OptVal<IsOptPath<T, P>, ValN<T, P>>;
```
