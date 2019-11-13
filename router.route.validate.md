<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/router](./router.md) &gt; [Route](./router.route.md) &gt; [validate](./router.route.validate.md)

## Route.validate property

This object specifies coercions and validators for variable / parameterized path components, e.g.

```
{
 id: {
         coerce: (x) => parseInt(x,10),
         validate: (x)=> x < 100
     }
}

```
This will first coerce the `id` route param to a number and then only allow the route to be matched if `id < 100`<!-- -->.

<b>Signature:</b>

```typescript
validate?: IObjectOf<RouteParamValidator>;
```