# Library: Closures

```lua
function islclosure(func: (...any?) -> (...any?))
```

Returns true if the function passed is made in lua, Returns false if made in C

Example:

```lua
  function lclosure()
     print('Hello, World!')
  end

  print(islclosure(lclosure)) --> true
  print(islclosure(coroutine.wrap)) --> false
```
