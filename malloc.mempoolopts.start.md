<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/malloc](./malloc.md) &gt; [MemPoolOpts](./malloc.mempoolopts.md) &gt; [start](./malloc.mempoolopts.start.md)

## MemPoolOpts.start property

Anchor index (byte address) inside the array buffer. The MemPool stores its internal state from the given address and heap space starts at least 32 bytes later (depending on chosen `align` value). Unlike allocator state variables, `start`<!-- -->\` cannot be saved inside the array buffer itself. If the ArrayBuffer is passed to other consumers they must use the same start value. MUST be multiple of 4.

<b>Signature:</b>

```typescript
start: number;
```
