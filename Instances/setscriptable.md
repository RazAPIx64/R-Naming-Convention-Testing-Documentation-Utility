# Library: Instances

```lua
 function setscriptable(Object: Instance, Property: string, State: boolean): boolean
```
Sets the given property to a scriptable if the property isn't already scriptable.
Find non-scriptable properties here: https://roblox.fandom.com/wiki/Category:Properties_that_are_not_scriptable

Example:
```lua
  local a = Instance.new('Frame');
  setscriptable(a, 'Name', false)
  print(isscriptable(a, 'Name')) --> false
  task.spawn(function() a.Name = 'Hello, World!' end) --> Throw exception
  setscriptable(a, 'Name', true);
  print(isscriptable(a, 'Name)) --> true

  local b = Instance.new('LocalScript');
  setscriptable(a, 'UniqueId', true)
  b.UniqueId = game:GetService('HttpService'):GenerateGUID(false)
```
