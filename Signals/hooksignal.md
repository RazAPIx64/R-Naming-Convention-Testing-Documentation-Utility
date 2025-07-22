# Library: Signals

```function
  function hooksignal(signal: RBXScriptSignal, callback: (...any?) -> (...any?))
```
Hooks a signals `:Connect()` Event with `callback`
Supports Binds

Example:

```lua
  local ok = 'What'
  local a = Instance.new('BindableEvent', game.GetService(game, 'ReplicatedStorage'));
  a.Event:Connect(function() return 'ok' end)
  print(firesignal(a)) --> 'ok'

  hooksignal(a.Event, function() return 'yes' end)
  print(firesignal(a)) --> 'yes'
```
