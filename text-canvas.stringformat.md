<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/text-canvas](./text-canvas.md) &gt; [StringFormat](./text-canvas.stringformat.md)

## StringFormat interface

<b>Signature:</b>

```typescript
export interface StringFormat 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [end](./text-canvas.stringformat.end.md) | <code>string</code> | Format end string (e.g. to ANSI reset or <code>&lt;/span&gt;</code>). |
|  [prefix](./text-canvas.stringformat.prefix.md) | <code>string</code> | Prefix for each canvas row / line result string |
|  [start](./text-canvas.stringformat.start.md) | <code>Fn&lt;number, string&gt;</code> | Function translating canvas character format codes to the actual output format. This function will only be called when needed, i.e. when a character's format is different than that of the previous. |
|  [suffix](./text-canvas.stringformat.suffix.md) | <code>string</code> | Suffix for each canvas row / line result string (e.g. linebreak) |
