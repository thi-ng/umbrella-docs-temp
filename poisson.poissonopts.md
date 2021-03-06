<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/poisson](./poisson.md) &gt; [PoissonOpts](./poisson.poissonopts.md)

## PoissonOpts interface

Options for [samplePoisson](./poisson.samplepoisson.md)<!-- -->.

<b>Signature:</b>

```typescript
export interface PoissonOpts 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [density](./poisson.poissonopts.density.md) | <code>DensityFunction &#124; number</code> | Density field function. Called for each new candidate point created by point generator and should return the poisson disc exclusion radius for the given point location. The related candidate point can only be placed if no other points are already existing within the given radius/distance. If this option is given as number, uses this value to create a uniform distance field. |
|  [index](./poisson.poissonopts.index.md) | <code>ISpatialSet&lt;ReadonlyVec&gt;</code> | Spatial indexing implementation for nearest neighbor searches of candidate points. Currently only  is available and must be pre-initialized to given dimensions prior to calling [samplePoisson](./poisson.samplepoisson.md)<!-- -->.<!-- -->The data structure is used to store all successful sample points (as keys) incl. their exclusion radius (as value).<!-- -->Furthermore, pre-seeding the data structure allows already indexed points to participate in the sampling process and act as exclusion zones. It also can be used as mechanism for progressive sampling, i.e. generating a large number of samples and distributing the process over multiple invocations of smaller sample sizes (see <code>max</code> option) to avoid long delays. |
|  [iter](./poisson.poissonopts.iter.md) | <code>number</code> | Number of random walk steps performed before giving up on a candidate point. Increasing this value improves overall quality. |
|  [jitter](./poisson.poissonopts.jitter.md) | <code>number</code> | Step distance for the random walk each failed candidate point is undergoing. This distance should be adjusted depending on overall sampling area/bounds. |
|  [max](./poisson.poissonopts.max.md) | <code>number</code> | Max number of samples to produce. Must be given, no default. |
|  [points](./poisson.poissonopts.points.md) | <code>PointGenerator</code> | Point generator function. Responsible for producing a new candidate point within user defined bounds using provided RNG. |
|  [quality](./poisson.poissonopts.quality.md) | <code>number</code> | Number of allowed failed consecutive candidate points before stopping entire sampling process (most likely due to not being able to place any further points). As with the <code>iter</code> param, increasing this value improves overall quality, especially in dense regions with small radii. |
|  [rnd](./poisson.poissonopts.rnd.md) | <code>IRandom</code> | Random number generator instance. |

