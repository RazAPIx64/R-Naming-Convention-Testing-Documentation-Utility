# Library: Scripts

```lua
 function getrunningscripts(): {Instance | LocalScript | ModuleScript | Script}
```

Returns all running scripts inside of `game` and running scripts parented to nil
LocalScripts that are parented to an Actor will automatically run under the Actor without the .Enabled property.

Example:

```lua
  for i,v in getrunningscripts() do
     print(v:GetFullName())
  end
```
