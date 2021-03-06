<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/router](./router.md) &gt; [BasicRouter](./router.basicrouter.md)

## BasicRouter class

<b>Signature:</b>

```typescript
export declare class BasicRouter implements INotify 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(config)](./router.basicrouter._constructor_.md) |  | Constructs a new instance of the <code>BasicRouter</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [config](./router.basicrouter.config.md) |  | <code>RouterConfig</code> |  |
|  [current](./router.basicrouter.current.md) |  | <code>RouteMatch &#124; undefined</code> |  |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [addListener(id, fn, scope)](./router.basicrouter.addlistener.md) |  |  |
|  [format(id, params, hash)](./router.basicrouter.format.md) |  | Returns a formatted version of given [RouteMatch](./router.routematch.md)<!-- -->, incl. any params. Throw an error if an invalid route <code>id</code> is provided. |
|  [format(match, hash)](./router.basicrouter.format_1.md) |  |  |
|  [handleRouteFailure()](./router.basicrouter.handleroutefailure.md) |  |  |
|  [matchRoute(curr, route)](./router.basicrouter.matchroute.md) |  |  |
|  [notify(event)](./router.basicrouter.notify.md) |  |  |
|  [removeListener(id, fn, scope)](./router.basicrouter.removelistener.md) |  |  |
|  [route(src)](./router.basicrouter.route.md) |  | Main router function. Attempts to match given input string against all configured routes. If none matches, falls back to default route. Before returning, triggers event with return value as well. |
|  [routeForID(id)](./router.basicrouter.routeforid.md) |  |  |
|  [start()](./router.basicrouter.start.md) |  |  |
|  [validateRouteParams(params, validators)](./router.basicrouter.validaterouteparams.md) |  |  |

