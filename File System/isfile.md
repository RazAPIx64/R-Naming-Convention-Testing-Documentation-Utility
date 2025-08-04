# Library: File System

```lua
function isfile(path: string): boolean
```
Checks if `path` is a file, (return true for file, return false for folder)

Example:
```lua
writefile('ok.txt', 'ok')
print(isfile('ok.txt')) --> true
makefolder('ok')
print(isfile('ok')) --> false
```
