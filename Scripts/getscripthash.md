# Library: Scripts

```lua
function getscripthash(script: LocalScript | ModuleScript | Script): string
```

Returns the script's hash by hashing the bytecode with sha-256 (Source), If **Source** is empty return an empty string.

**WARNING**: Using script:GetHash() is inaccurate, and does not work on ModuleScripts.

Example:
```lua
 local Scr = Instance.new('LocalScript', game.Players.LocalPlayer.PlayerScripts);
 print(getscripthash(Scr)) --> ''

 local Scr = Instance.new('LocalScript', game.Players.LocalPlayer.PlayerScripts);
 Scr.Source = [[print("Source?")]]
 print(getscripthash(Scr)) --> hashed sha-256 bytecode
```
