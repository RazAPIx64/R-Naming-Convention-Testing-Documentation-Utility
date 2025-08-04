# Library: File System

```lua
function writefile(path: string, content: string)
```
Creates a `file` inside of the workspace folder, with it's content being `content`

Example:
```lua
 writefile('Hello.txt', 'Hello, World!')
 print(isfile('Hello.txt')) --> true

 local a,b = pcall(function()
     writefile('Hello.py', 'def ok(): #??')   
 end)

 print(a) --> false, Should return an error when trying to create a file that can have malicious impacts on the users PC
```
