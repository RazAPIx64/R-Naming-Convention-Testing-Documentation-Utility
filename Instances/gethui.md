# Library: Instances

```lua
  function gethui(): BasePlayerGui | Folder
```
Returns a Hidden User-Interface Container parented to CoreGui, or RobloxGui
The Instance that `gethui` returns should be a `BasePlayerGui` or `Folder`
It must be protected from common detection methods (DescendantAdded, ChildAdded)

Example:

```lua
  local a = Instance.new('ScreenGui');
  a.Parent = gethui()
```
