# Library: Misc

```lua
function lz4decompress(data: string, size: number): string
```
Decompresses a string (`data`) using lz4 within the given (`size`)
Example:

```lua
local a = "Hello, world! Hello, world!"
local b = lz4compress(a)
print(lz4decompress(b, #a)) --> "Hello, world! Hello, world!"
```
