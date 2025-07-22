# Library: Scripts

```lua
  function getscriptbytecode(script: LocalScript | ModuleScript | Script): string
```

Returns the bytecode inside of a LuaSourceContainer (LocalScript, ModuleScript, Script), mostly Scripts that have their RunContext set to Client
The `script` arg must have the Property: **Source**

If **Source** is empty, return an empty string

Example:

```lua
  local LocalScript = Instance.new('LocalScript', game.GetService(game, 'Players').LocalPlayer['PlayerScripts']);
  print(getscriptbytecode(LocalScript)) --> ''

  local LocalScript2 = Instance.new('LocalScript', game.GetService(game, 'Players').LocalPlayer['PlayerScripts']);
  LocalScript2.Source = [[
     print("Hello") 
  ]]
  print(getscriptbytecode(LocalScript2)) --> Bytecode of the script from it's Source
```
