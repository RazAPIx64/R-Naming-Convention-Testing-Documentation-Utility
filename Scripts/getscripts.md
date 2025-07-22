# Library: Scripts

```lua
function getscripts(): {LocalScript | ModuleScript | Script}
```

Returns all scripts available in the `game`, and returns all scripts parented to nil

Example:

```lua
   for i,v in getscripts() do
      print(v:GetFullName())
   end
```
