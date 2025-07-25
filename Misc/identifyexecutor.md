# Library: Misc

```lua
function identifyexecutor(): (string, string) -- Name, Version
```
:warning:`Alias: getexecutorname`

Returns 2 strings representing the executors name and version

Example:

```lua
local ExecutorName, ExecutorVersion = identifyexecutor()
print(ExecutorName) --> Executor
print(ExecutorVersion) --> v1.0.0

print(ExecutorName, ExecutorVersion) --> Executor v1.0.0
```
