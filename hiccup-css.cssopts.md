<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/hiccup-css](./hiccup-css.md) &gt; [CSSOpts](./hiccup-css.cssopts.md)

## CSSOpts interface

Config options supported by [css](./hiccup-css.css.md) and its helper functions.

<b>Signature:</b>

```typescript
export interface CSSOpts 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [autoprefix](./hiccup-css.cssopts.autoprefix.md) | <code>string[] &#124; Set&lt;string&gt;</code> | Array or set of properties to prefix automatically. If given, each listed property will be prefixed with values given under <code>vendors</code>.<!-- -->By default, no properties are prefixed. |
|  [depth](./hiccup-css.cssopts.depth.md) | <code>number</code> | Current tree depth. Internal use only. Ignore. |
|  [fns](./hiccup-css.cssopts.fns.md) | <code>IObjectOf&lt;FnAny&lt;RuleFn&gt;&gt;</code> | Dictionary object for JSON-<!-- -->&gt;<!-- -->CSS conversion Maps keys to rule functions. See quoted-functions.ts |
|  [format](./hiccup-css.cssopts.format.md) | <code>Format</code> | CSS output format config. Two presets are included: COMPACT (default), PRETTY |
|  [scope](./hiccup-css.cssopts.scope.md) | <code>string</code> | Optional scoping suffix for CSS classes |
|  [vendors](./hiccup-css.cssopts.vendors.md) | <code>string[]</code> | Prefix strings for props under <code>autoprefix</code> Defaults to <code>DEFAULT_VENDORS</code> object. |

