# Library: Closures

```lua
function loadstring(source: string, chunk: string?): (...any?) -> (...any?) | string?
```
Executes luau code (`source`) as bytecode by compiling the source into bytecode and loading it.
:warning: **WARNING**: You must load the global environment & variables from the environment when making this function.

`chunk` is used as debug information for errors. if nil, return a randomized string or return an empty string

Example:
```lua
local a,err = loadstring('return "Half The Plot"')
print(a()) --> Half The Plot

local c,err = loadstring('return ... + 1'); -- ... is represented as the first argument of the function that is returned by the compiler
print(c(1)) --> 2

local f,err = loadstring('Error()')
print(f, err) --> attempt to call a nil value
```
