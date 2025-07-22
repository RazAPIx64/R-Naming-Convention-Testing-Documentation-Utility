# Library: Instances

```lua
 function setscriptable(Object: Instance, Property: string, Value: boolean?): boolean
```
Sets the given property if scriptable (Equivalent to Object[Property] = Value), Returns whether the property was scriptable prior to changing it.

Example:
```lua
  local a = Instance.new('Frame');
  setscriptable(a, 'Name', 'Hello, World!')
  print(a.Name) --> Hello, World!

  local b = Instance.new('LuaSourceContainer');
  setscriptable(a, 'UniqueId', 0) --> Throw exception (Property is not scriptable)
```
