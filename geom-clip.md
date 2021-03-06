<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/geom-clip](./geom-clip.md)

## geom-clip package

## Variables

|  Variable | Description |
|  --- | --- |
|  [liangBarsky2](./geom-clip.liangbarsky2.md) | Performs Liang-Barsky clipping of the line segment with endpoints <code>a</code>, <code>b</code> against the clipping rect defined by <code>min</code> and <code>max</code>. The optional <code>ca</code> and <code>cb</code> vectors can be given to store the result (clipped points). If omitted creates new vectors. Returns a tuple of <code>[ca, cb, a, b]</code>, where the latter two values represent the normalized distances of the clipped points relative to original given line segment. Returns <code>undefined</code> iff the line lies completely outside the rect.<!-- -->- [https://en.wikipedia.org/wiki/Liang%E2%80%93Barsky\_algorithm](https://en.wikipedia.org/wiki/Liang%E2%80%93Barsky_algorithm) - [https://github.com/thi-ng/c-thing/blob/master/src/geom/clip/liangbarsky.c](https://github.com/thi-ng/c-thing/blob/master/src/geom/clip/liangbarsky.c) |
|  [sutherlandHodgeman](./geom-clip.sutherlandhodgeman.md) | Extended version of Sutherland-Hodgeman convex polygon clipping supporting any convex boundary polygon (not only rects). Returns new array of clipped vertices.[https://en.wikipedia.org/wiki/Sutherland%E2%80%93Hodgman\_algorithm](https://en.wikipedia.org/wiki/Sutherland%E2%80%93Hodgman_algorithm) |

