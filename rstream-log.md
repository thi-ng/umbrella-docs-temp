<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/rstream-log](./rstream-log.md)

## rstream-log package

## Classes

|  Class | Description |
|  --- | --- |
|  [Logger](./rstream-log.logger.md) |  |

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [ILogger](./rstream-log.ilogger.md) |  |
|  [LogEntry](./rstream-log.logentry.md) |  |
|  [LogEntryObj](./rstream-log.logentryobj.md) |  |

## Variables

|  Variable | Description |
|  --- | --- |
|  [formatJSON](./rstream-log.formatjson.md) |  |
|  [formatObject](./rstream-log.formatobject.md) |  |
|  [formatString](./rstream-log.formatstring.md) |  |
|  [isoDate](./rstream-log.isodate.md) |  |
|  [maskSecrets](./rstream-log.masksecrets.md) | Takes an array of regex patterns and optional <code>mask</code> string. Returns transducer which replaces all found pattern occurrences with <code>mask</code>. Intended to be used in combination / after <code>formatString()</code> to avoid leaking of sensitive information via logged messages.
```ts
logger.transform(
  formatString(),
  maskSecrets([/(?<=[A-Z0-9_]\=)\w+/g])
).subscribe(
  writeConsole()
);

logger.info("logged in USER=toxi, using TOKEN=123456");
// [INFO] logger-0: logged in USER=****, using TOKEN=****

```
 |
|  [matchID](./rstream-log.matchid.md) |  |
|  [maxLevel](./rstream-log.maxlevel.md) |  |
|  [minLevel](./rstream-log.minlevel.md) |  |
|  [onlyLevel](./rstream-log.onlylevel.md) |  |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [BodyFormat](./rstream-log.bodyformat.md) |  |
|  [DateFormat](./rstream-log.dateformat.md) |  |
