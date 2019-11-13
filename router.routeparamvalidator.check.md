<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/router](./router.md) &gt; [RouteParamValidator](./router.routeparamvalidator.md) &gt; [check](./router.routeparamvalidator.check.md)

## RouteParamValidator.check property

Optional arbitrary value validation. If any validator returns non-true result, the currently checked route becomes unmatched/invalid and the router continues checking other routes.

<b>Signature:</b>

```typescript
check: Fn<any, boolean>;
```