<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@thi.ng/system](./system.md) &gt; [System](./system.system.md) &gt; [start](./system.system.start.md)

## System.start() method

Initializes all system components in dependency order. If any component's `start()` method returns false, system start up will be stopped and this method returns false itself.

Also any errors thrown during child component startup will not be intercepted.

<b>Signature:</b>

```typescript
start(): Promise<boolean>;
```
<b>Returns:</b>

`Promise<boolean>`

