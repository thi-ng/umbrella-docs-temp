<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/hdom](./hdom.md) &gt; [createElement](./hdom.createelement.md)

## createElement variable

Creates a new DOM element of type `tag` with optional `attribs`<!-- -->. If `parent` is not `null`<!-- -->, the new element will be inserted as child at given `insert` index. If `insert` is missing, the element will be appended to the `parent`<!-- -->'s list of children. Returns new DOM node.

If `tag` is a known SVG element name, the new element will be created with the proper SVG XML namespace.

<b>Signature:</b>

```typescript
createElement: (parent: Element, tag: string, attribs?: any, insert?: number | undefined) => Node
```
