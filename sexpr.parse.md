<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/sexpr](./sexpr.md) &gt; [parse](./sexpr.parse.md)

## parse variable

Takes a `src` string or [Token](./sexpr.token.md) iteratable and parses it into an AST, then returns tree's root node. Throws [ParseError](./sexpr.parseerror.md) if the token order causes illegal nesting. The error includes `line` and `column` information of the offending token.

<b>Signature:</b>

```typescript
parse: (src: string | Iterable<Token>, opts?: Partial<SyntaxOpts> | undefined) => Root
```
