# Library: Cache

```lua
  function iscached(Object: Instance)
```
Checks if a `Instance`/`Object` is in the Internal Instance Cache

Example:
```lua
 local a = Instance.new('LocalScript')
 cache.iscached(a) -- true
 cache.invalidate(a)
 cache.iscached(a) -- false
```
