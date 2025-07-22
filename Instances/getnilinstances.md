# Library: Instances

```lua
 function getnilinstances(): {Instance}
```

Returns all Instances parented to `nil`
**WARNING**: Using game.DescendantRemoving only means that you are getting Instances that have been parented to `game`, and then have their Parent set to `nil`

Example:
```lua
  for i,v in getnilinstances() do
     print(v.Parent) --> nil
  end
```
