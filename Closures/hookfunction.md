# Library: Closures

```lua
function hookfunction(Function1: (...any?) -> (...any?))
```
Replaces the first function passed with the second one including the environments of the functions

Example:
```lua
 function ok() return 'Not Hooked' end
 function now() return 'Hooked' end

 hookfunction(ok, now)
 print(ok()) --> Hooked
```
