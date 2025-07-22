# Library: Scripts

```lua
 function getloadedmodules(excludeCore: boolean): {ModuleScript | CoreScript}
```

Returns all loaded/required modules & active CoreScripts inside of `game`

Example:

```lua
  for i,v in getloadedmodules(true)
    print(v:GetFullName())
  end
```
