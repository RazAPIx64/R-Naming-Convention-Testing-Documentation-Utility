# Library: Misc

```lua
function lz4compress(data: string): string
```
Compresses a string (`data`) using lz4 compression

Example:
```lua
  local a = 'HelloWorldByTheCrowd'
  print(#a) --> 5
  print(#lz4compress(a)) --> 32
```
