<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/hdom](./hdom.md) &gt; [equiv](./hdom.equiv.md)

## equiv variable

Customized version [equiv](./equiv.equiv.md) which takes `__diff` attributes into account (at any nesting level). If an hdom element's attribute object contains `__diff: false`<!-- -->, the object will ALWAYS be considered unequal, even if all other attributes in the object are equivalent.

<b>Signature:</b>

```typescript
equiv: (a: any, b: any) => boolean
```
