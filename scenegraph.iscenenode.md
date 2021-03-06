<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/scenegraph](./scenegraph.md) &gt; [ISceneNode](./scenegraph.iscenenode.md)

## ISceneNode interface

<b>Signature:</b>

```typescript
export interface ISceneNode<T extends ISceneNode<T>> extends IID<string> 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [children](./scenegraph.iscenenode.children.md) | <code>T[]</code> |  |
|  [invMat](./scenegraph.iscenenode.invmat.md) | <code>Mat</code> |  |
|  [mat](./scenegraph.iscenenode.mat.md) | <code>Mat</code> |  |
|  [parent](./scenegraph.iscenenode.parent.md) | <code>Nullable&lt;T&gt;</code> |  |

## Methods

|  Method | Description |
|  --- | --- |
|  [childForPoint(p)](./scenegraph.iscenenode.childforpoint.md) |  |
|  [containsLocalPoint(\_)](./scenegraph.iscenenode.containslocalpoint.md) |  |
|  [draw(ctx)](./scenegraph.iscenenode.draw.md) |  |
|  [mapGlobalPoint(p)](./scenegraph.iscenenode.mapglobalpoint.md) |  |
|  [mapLocalPointToNode(dest, p)](./scenegraph.iscenenode.maplocalpointtonode.md) |  |
|  [update()](./scenegraph.iscenenode.update.md) |  |

