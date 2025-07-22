# Library: Cache

```lua
 function replace(Object1: Instance, Object2: Instance)
```
Replaces an `Instance`/`Object` inside of the Internal Instance Cache with another `Instance`
Example:
```lua
  local LocalScript = Instance.new('LocalScript');
  local ModuleScript = Instance.new('ModuleScript');
  
  cache.replace(LocalScript, ModuleScript)
  
  print(LocalScript) --> ModuleScript 
```
