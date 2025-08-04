# Library: File System

```lua
function appendfile(path: string, content: string): ()
```
Appends `content` to the last line/end of the file (`path`)
Creates the file if it does not exist.

Example:
```lua
writefile('JivinchciAllOnMe.txt', 'Available Players:\n')

for _, player in game.Players:GetPlayers() do
   appendfile('JivinchciAllOnMe.txt', player.DisplayName .. '\n')
end
```
