# Library: File System

```lua
function isfolder(path: string): boolean
```
Checks if `path` is a folder (return true if folder, return false if file)

Example:
```lua
makefolder('ok')
print(isfolder('ok')) --> true
writefile('ok.txt', 'ok')
print(isfolder('ok.txt')) --> false
```
