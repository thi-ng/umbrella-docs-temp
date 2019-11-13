<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/strings](./strings.md)

## strings package

## Functions

|  Function | Description |
|  --- | --- |
|  [charRange(from, to)](./strings.charrange.md) | Yields iterator of characters \[<code>from</code>..<code>to</code>\] (inclusive). Uses reverse ordering if <code>to</code> &lt; <code>from</code>. |

## Variables

|  Variable | Description |
|  --- | --- |
|  [B16](./strings.b16.md) | 16bit binary conversion preset. |
|  [B32](./strings.b32.md) | 32bit binary conversion preset. |
|  [B8](./strings.b8.md) | 8bit binary conversion preset. |
|  [bits](./strings.bits.md) |  |
|  [bytes](./strings.bytes.md) |  |
|  [camel](./strings.camel.md) | Converts a kebab-case or snake\_case string into CamelCase. Uses <code>-</code> as default delimiter. |
|  [capitalize](./strings.capitalize.md) | String formatter which capitalizes first character. |
|  [center](./strings.center.md) | Returns stringer which pads given input with <code>ch</code> (default: space) on both sides and returns fixed width string of given <code>lineWidth</code>. Returns string of only pad characters for any <code>null</code> or <code>undefined</code> values. If the string version of an input is &gt; <code>lineWidth</code>, no centering is performed, but the string will be truncated to <code>lineWidth</code>.<!-- -->Note: The padding string can contain multiple characters.
```ts
center(20, "<>")(wrap(" ")("thi.ng"))
// "<><><> thi.ng <><><>"

```
 |
|  [float](./strings.float.md) | Returns <code>Stringer</code> which formats numbers to given precision. Exceptions:<!-- -->- NaN =<!-- -->&gt; "NaN" - Infinity =<!-- -->&gt; "+/-∞" |
|  [floatFixedWidth](./strings.floatfixedwidth.md) | Similar to <code>float</code>, returns <code>Stringer</code> which formats numbers to given character width &amp; precision. Uses scientific notation if needed.<!-- -->Default precision: 3 fractional digits |
|  [format](./strings.format.md) |  |
|  [grams](./strings.grams.md) |  |
|  [hstr](./strings.hstr.md) | Formats given value <code>x</code> as Fortran style Hollerith string.
```ts
hstr("abc")  // "3Habc"
hstr(123.45) // "6H123.45"
hstr("")     // "0H"
hstr(null)   // ""

```
[https://en.wikipedia.org/wiki/Hollerith\_constant](https://en.wikipedia.org/wiki/Hollerith_constant) |
|  [kebab](./strings.kebab.md) | Converts a CamelCase string into kebab case, with optional custom delimiter (<code>-</code> by default).<!-- -->TODO: Switch back to currently broken Regex w/ positive lookbehind, once avail in FF &amp; Safari (currently TC39 stage 4)[https://github.com/tc39/proposal-regexp-lookbehind](https://github.com/tc39/proposal-regexp-lookbehind)
```ts
kebab("FooBar23Baz");
// "foo-bar23-baz"

```
 |
|  [lower](./strings.lower.md) | Lowercase string formatter. |
|  [maybeParseFloat](./strings.maybeparsefloat.md) |  |
|  [maybeParseInt](./strings.maybeparseint.md) |  |
|  [meters](./strings.meters.md) |  |
|  [padLeft](./strings.padleft.md) |  |
|  [padRight](./strings.padright.md) |  |
|  [percent](./strings.percent.md) | Returns <code>Stringer</code> which formats given fractions as percentage (e.g. <code>0.1234 =&gt; 12.34%</code>). |
|  [radix](./strings.radix.md) | Returns a <code>Stringer</code> which formats given numbers to <code>radix</code>, <code>len</code> and with optional prefix (not included in <code>len</code>). |
|  [repeat](./strings.repeat.md) |  |
|  [seconds](./strings.seconds.md) |  |
|  [slugify](./strings.slugify.md) | Based on: [https://medium.com/@matthagemann/the-ultimate-way-to-slugify-a-url-string-in-javascript-b8e4a0d849e1](https://medium.com/@matthagemann/the-ultimate-way-to-slugify-a-url-string-in-javascript-b8e4a0d849e1) |
|  [snake](./strings.snake.md) | Short for <code>kebab</code> using <code>_</code> as delimiter. |
|  [splice](./strings.splice.md) | Forms a new strings which inserts given <code>insert</code> string into <code>src</code> string at <code>from</code> position and appends remaining <code>src</code> chars from original <code>to</code> position. If <code>from</code> and <code>to</code> are equal (<code>to</code> by default is), the operation is a pure insertion. If not, then some chars from <code>src</code> will be removed in the new string. If either position is negative, it'll be considered relative to the end of the <code>src</code>. |
|  [truncate](./strings.truncate.md) |  |
|  [truncateLeft](./strings.truncateleft.md) |  |
|  [U16](./strings.u16.md) | 16bit hex conversion preset. Assumes unsigned inputs. |
|  [U24](./strings.u24.md) | 24bit hex conversion preset. Assumes unsigned inputs. |
|  [U32](./strings.u32.md) | 32bit hex conversion preset. Assumes unsigned inputs. |
|  [U64](./strings.u64.md) | 64bit hex conversion preset (2x 32bit ints) Assumes unsigned inputs. |
|  [U8](./strings.u8.md) | 8bit hex conversion preset. Assumes unsigned inputs. |
|  [units](./strings.units.md) |  |
|  [upper](./strings.upper.md) | Uppercase string formatter. |
|  [wrap](./strings.wrap.md) | Returns a <code>Stringer</code> which wrap inputs with given <code>pad</code> string on both sides. |
|  [Z2](./strings.z2.md) | Zero-padded 2 digit formatter. |
|  [Z3](./strings.z3.md) | Zero-padded 3 digit formatter. |
|  [Z4](./strings.z4.md) | Zero-padded 4 digit formatter. |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [Stringer](./strings.stringer.md) |  |
