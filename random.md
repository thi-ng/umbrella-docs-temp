<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/random](./random.md)

## random package

## Classes

|  Class | Description |
|  --- | --- |
|  [ARandom](./random.arandom.md) |  |
|  [Smush32](./random.smush32.md) |  |
|  [SystemRandom](./random.systemrandom.md) |  |
|  [XorShift128](./random.xorshift128.md) |  |
|  [XorWow](./random.xorwow.md) |  |
|  [Xoshiro128](./random.xoshiro128.md) |  |
|  [XsAdd](./random.xsadd.md) |  |

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [IRandom](./random.irandom.md) |  |
|  [ISeedable](./random.iseedable.md) |  |

## Variables

|  Variable | Description |
|  --- | --- |
|  [randomBytes](./random.randombytes.md) | Fills given byte array with random values. Wrapper for <code>crypto.getRandomValues()</code> with automatic fallback to using <code>Math.random</code> if platform doesn't provide global crypto instance. |
|  [randomID](./random.randomid.md) | Generates and returns a random string of <code>len</code> characters (default 4), plus optional given <code>prefix</code> and using only provided <code>syms</code> characters (default lowercase a-z). |
|  [SYSTEM](./random.system.md) |  |
|  [uuidv4Bytes](./random.uuidv4bytes.md) |  |
|  [weightedRandom](./random.weightedrandom.md) | Returns a no-arg function which produces a random choice of given weighted <code>choices</code> and using given [IRandom](./random.irandom.md) instance (default [SYSTEM](./random.system.md)<!-- -->. If <code>weights</code> are given, it must be the same size as <code>choices</code>. If omitted, each choice will have same probability.[https://www.electricmonk.nl/log/2009/12/23/weighted-random-distribution/](https://www.electricmonk.nl/log/2009/12/23/weighted-random-distribution/) |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [ISeedableRandom](./random.iseedablerandom.md) |  |

