# Library: Closures

```lua
function newcclosure(func: (...any?) -> (...any?))
```
Returns the function wrapped in a C Closure

**WARNING**: Externals may use coroutines to make this function, but they cannot be yielded, and they cannot be recursive
Example (Without Coroutines):

```lua
  a = newcclosure(function(name)
     print('Hello,', name)
  end)

  print(iscclosure(a)) --> true
  print(islclosure(a)) --> false
```

Example (With Coroutines):

```lua
local example

example = function()
    example()
end

example = newcclosure(example)
example() --> Will error due to coroutine.wrap not being recursive
```
