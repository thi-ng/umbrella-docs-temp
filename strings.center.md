<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/strings](./strings.md) &gt; [center](./strings.center.md)

## center variable

Returns stringer which pads given input with `ch` (default: space) on both sides and returns fixed width string of given `lineWidth`<!-- -->. Returns string of only pad characters for any `null` or `undefined` values. If the string version of an input is &gt; `lineWidth`<!-- -->, no centering is performed, but the string will be truncated to `lineWidth`<!-- -->.

Note: The padding string can contain multiple characters.

<b>Signature:</b>

```typescript
center: (lineWidth: number, pad?: string | number) => Stringer<any>
```

## Example


```ts
center(20, "<>")(wrap(" ")("thi.ng"))
// "<><><> thi.ng <><><>"

```

