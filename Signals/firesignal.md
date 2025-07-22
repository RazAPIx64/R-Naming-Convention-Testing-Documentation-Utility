# Library: Signals

```lua
  function firesignal(signal: RBXScriptSignal, ...: any?)
```
Fires a RBXScriptSignal from it's .Event Method, The equivalent of

```lua
  for i,v in getconnections(Bind.Event) do
     local Function = v.Function
     if Function then
         task.spawn(Function, ...)
       end
    end
```

Example:

```lua
  local Bind = Instance.new('BindableEvent');
  Bind.Event:Connect(function()
     return 'ok' 
  end)
  print(firesignal(Bind.Event)) --> 'ok'
  local Bind2 = Instance.new('BindableEvent');
  Bind2.Event:Connect(function(s)
     return s
  end)
  print(firesignal(Bind2.Event, 'Hello, World!')) --> 'Hello, World!'
```
