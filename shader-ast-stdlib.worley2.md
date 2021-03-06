<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/shader-ast-stdlib](./shader-ast-stdlib.md) &gt; [worley2](./shader-ast-stdlib.worley2.md)

## worley2 variable

Higher order function. Computes 2D Worley noise using provided distance function. The returned function takes 2 args: position and jitter amount, the latter in \[0..1\] interval. Returns noise components as vec2, with the x component containing the distance from closest simplex center and y the noise value. The vector components can be used individually or combined (e.g. `noise.y - noise.x`<!-- -->)...

Based on implementation by Stefan Gustavson: [http://webstaff.itn.liu.se/\~stegu/GLSL-cellular/GLSL-cellular-notes.pdf](http://webstaff.itn.liu.se/~stegu/GLSL-cellular/GLSL-cellular-notes.pdf)

<b>Signature:</b>

```typescript
worley2: (distFn: import("@thi.ng/api").Fn2<import("@thi.ng/shader-ast").Term<"vec3">, import("@thi.ng/shader-ast").Term<"vec3">, import("@thi.ng/shader-ast").FnCall<"vec3">>) => import("@thi.ng/shader-ast").TaggedFn2<"vec2", "float", "vec2">
```
