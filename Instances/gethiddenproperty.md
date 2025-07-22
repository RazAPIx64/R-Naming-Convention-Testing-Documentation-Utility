# Library: Instances

```lua
 function gethiddenproperty(Object: Instance, Property: string): (any, boolean)
```
Returns a value of a hidden `Property` in `Object`, which cannot be indexed normally as the property is hidden from the user.

Example:
```lua
 local a = Instance.new('VirtualInputManager');
 print(select(1, gethiddenproperty(a, 'AdditionalLuaState')) --> '', true
 local b = Instance.new('Folder');
 b.RobloxLocked = true

 print(select(1, gethiddenproperty(b, 'Name'))) --> Folder, false
 print(select(1, gethiddenproperty(b, 'RobloxLocked'))) --> true, true
```
