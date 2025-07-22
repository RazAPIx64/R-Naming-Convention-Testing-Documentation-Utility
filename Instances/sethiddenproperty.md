# Library: Instances

```lua
function sethiddenproperty(Object: Instance, Property: string, Value: any): boolean
```

Sets the value of a hidden `Property` in `Object`, which cannot be assigned normally due to being hidden from the user.
Returns `true` if the property was successfully set, otherwise `false`.

Example:

```lua
local a = Instance.new('VirtualInputManager');
sethiddenproperty(a, 'AdditionalLuaState', 'hi') --> true
print(gethiddenproperty(a, 'AdditionalLuaState')) --> hi

local b = Instance.new('Folder')
sethiddenproperty(b, 'RobloxLocked', true) --> true
print(gethiddenproperty(b, 'RobloxLocked')) --> true, true

local c = Instance.new('Folder')
sethiddenproperty(c, 'NonExistentHiddenProperty', 123) --> false (property does not exist)
```
