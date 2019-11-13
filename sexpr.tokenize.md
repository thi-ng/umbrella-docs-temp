<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/sexpr](./sexpr.md) &gt; [tokenize](./sexpr.tokenize.md)

## tokenize() function

Yields iterator of `Token`<!-- -->s (incl. location info) from `src` string (or from a \*\*characterwise\*\* iterable). Scope and string delimiters and whitespace characters can be configured via given `opts`<!-- -->. By default `DEFAULT_SYNTAX` is used.

 SyntaxOpts  Token

<b>Signature:</b>

```typescript
export declare function tokenize(src: Iterable<string>, opts?: Partial<SyntaxOpts>): Generator<Token, void, unknown>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  src | <code>Iterable&lt;string&gt;</code> |  |
|  opts | <code>Partial&lt;SyntaxOpts&gt;</code> |  |

<b>Returns:</b>

`Generator<Token, void, unknown>`
