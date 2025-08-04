# Library: File System

```lua
function listfiles(path: string): table
```
Lists files ***and folders*** inside of `path`.
Yes, this should also list folders inside of `path`

If `path` is a empty string, list all files/folders inside of the executor's workspace folder.
Example:
```lua
 writefile('dir.txt', 'ok')
 for i, v in listfiles('') do
   if v then print('File found: ', v) end --> File found: dir.txt
 end
```
