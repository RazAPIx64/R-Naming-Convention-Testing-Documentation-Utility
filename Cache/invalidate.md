# Library: Cache

```lua
  function invalidate(Object: Instance)
```
Invalidates an `Instance`/`Object` inside of the Internal Instance Cache

Example:
```lua
 local a = Instance.new('LocalScript', game);
 cache.invalidate(game:FindFirstChild('LocalScript'));
 print(a == game:FindFirstChild('LocalScript')) --> false
```
