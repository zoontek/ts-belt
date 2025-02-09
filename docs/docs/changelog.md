---
id: changelog
title: Changelog
---

### `v3.4.1`

- 🐛 fixed `F.makeControlledThrottle`
- 🐛 fixed `F.makeControlledDebounce`

⬆️ The `invoke` method was accepting only one argument.

### `v3.4.0`

- 🐛 fixed the internal implementation for comparing objects
- ✨ added `D.set`

### `v3.3.0`

- ♻️ all tuples are now `readonly`
- 🗑 `D.prop` has been deprecated (please use either `D.get` or `D.getUnsafe`)
- ✨ added `A.flip`
- ✨ added `F.tap`
- ✨ added `F.debounce`
- ✨ added `F.makeControlledDebounce`
- ✨ added `F.throttle`
- ✨ added `F.makeControlledThrottle`

### `v3.2.0`

This version provides much better support for the point-free style. For instance, the following should not throw an error in TypeScript:

```typescript
A.reduce([1, 2, 3], 0, N.add)
A.reduce(['hello', 'world'], '', S.concat)
A.filter(['hello', 'world'], S.startsWith('h'))
```

- ✨ added `O.tap`
- ✨ added `R.tap`
- ✨ added `A.tap`

### `v3.1.1`

- 🐛 fixed arguments order of `A.*WithIndex` → `(index, value)` and `D.*WithKey` → `(key, value)`  functions

### `v3.1.0`

- 🐛 fixed `S.head` return type
- ✨ added `S.trimEnd`
- ✨ added `S.trimStart`
- ✨ added `S.last`

### `v3.0.1`

- 🐛 fixed `A.uniqBy` implementation

### `v3.0.0`

Initial `v3` implementation.
