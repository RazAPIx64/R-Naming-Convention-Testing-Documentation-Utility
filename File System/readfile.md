# Library: File System

```lua
function readfile(path: string): string
```
Returns the `content` from a `file`
(Please remember to hence the word read`file`, and not read`folder`.)

Example:

```lua
writefile('Hello.txt', 'Hello, World!');
print(readfile('Hello.txt')) --> Hello, World!
```
