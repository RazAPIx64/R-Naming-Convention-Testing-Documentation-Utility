# Library: Instances

```lua
 function isscriptable(Object: Instance, Property: string): boolean
```

Checks if the given `Property` can be indexed and can be modified (Properties without the Not Scriptable tag)
If true, The `Property` can be modified and indexed normally, if false, The `Property` cannot be modified and indexed normally

Example:
```lua
 local a = Instance.new('LuaSourceContainer');
 print(isscriptable(a, 'IsDifferentFromFileSystem')) --> false, Property cannot be indexed and cannot be modified
 print(isscriptable(Instance.new('Frame'), 'Name')) --> true, Property can be indexed and can be modified

 local b = Instance.new('LocalScript')
 print(isscriptable(b, 'UniqueId')) --> false, Property cannot be modified 
```
