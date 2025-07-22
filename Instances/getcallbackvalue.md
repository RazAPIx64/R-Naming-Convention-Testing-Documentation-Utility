# Library: Instances

```lua
  function getcallbackvalue(Object: Instance, Property: string): function?
```

Returns the function assigned to a callback property of `Object`, which cannot be indexed normally

Example:

```lua
  local a = Instance.new('BindableFunction')
  a.OnInvoke = function()
     return 'Drakon!'
  end

  print(a.OnInvoke) --> Error
  print(type(getcallbackvalue(a, 'OnInvoke'))) --> function
 ```
