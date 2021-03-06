<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream-query](./rstream-query.md) &gt; [TripleStore](./rstream-query.triplestore.md) &gt; [addPatternQuery](./rstream-query.triplestore.addpatternquery.md)

## TripleStore.addPatternQuery() method

Creates a new query subscription from given SPO pattern. Any `null` values in the pattern act as wildcard selectors and any other value as filter for the given triple component. E.g. the pattern `[null, "type", "person"]` matches all triples which have `"type"` as predicate and `"person"` as object. Likewise the pattern `[null, null, null]` matches ALL triples in the graph.

By default, the returned rstream subscription emits sets of matched triples. If only the raw triple IDs are wanted, set `emitTriples` arg to `false`<!-- -->.

<b>Signature:</b>

```typescript
addPatternQuery(pattern: Pattern, id?: string): ISubscribable<Triples>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  pattern | <code>Pattern</code> |  |
|  id | <code>string</code> |  |

<b>Returns:</b>

`ISubscribable<Triples>`

