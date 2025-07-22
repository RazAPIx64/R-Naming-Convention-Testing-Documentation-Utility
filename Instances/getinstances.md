# Library: Instances

```lua
  function getinstances(): {Instance}
```

Returns all Instances available inside of `game` and parented to nil

Example:
```lua
  for i,v in getinstances() do
    print(v:GetFullName())
  end
```
