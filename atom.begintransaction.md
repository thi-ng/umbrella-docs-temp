<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/atom](./atom.md) &gt; [beginTransaction](./atom.begintransaction.md)

## beginTransaction variable

Like [defTransacted](./atom.deftransacted.md)<!-- -->, but immediately starts new transaction as well, i.e. same as `defTransacted(state).begin()`<!-- -->.

<b>Signature:</b>

```typescript
beginTransaction: <T>(parent: IAtom<T>) => Transacted<T>
```