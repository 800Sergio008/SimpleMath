# SimpleMath

## Description
A pure Luau implementation of mathematical functions, constants, and utilities built without reliance on Roblox's native `math` library. Written with strict dynamic typing `--!strict` and high precision approximations.

## Capabilities
- Strict Type Checking: built with `--!strict` mode for robust integration
- Zero External Dependencies: implements algorithms (Taylor series, Newton-Raphson, Polynomial Approximations) from scratch
- Comprehensive API: standard math operations, logarithmic and exponential calculations, trigonometry, and range utilities
- Immutable: prevented runtime mutation

---
---
## Installation
1. Copy the contents of `SimpleMath.luau` into a ModuleScript inside your Roblox project or Luau application
2. Require the module whenever needed:
```luau
local SimpleMath = require(path.to.SimpleMath)
```
### Optional
3. Swap Roblox's `math` library with `SimpleMath`:
```luau
local SimpleMath = require(path.to.SimpleMath)

local math = SimpleMath
```
## Example
```luau
local SimpleMath = require(path.to.SimpleMath)

-- Constants
print(SimpleMath.PI) -- 3.1415926...

-- Standard operations
print(SimpleMath.Round(7.2081, 2)) -- 7.20
print(SimpleMath.Sqrt(16)) -- 4

-- Trigonometry
print(SimpleMath.Sin(Math.PI / 2)) -- 1

-- Advanced Utilities
print(SimpleMath.Lerp(0, 100, 0.5)) -- 50
print(SimpleMath.Clamp(15, 0, 10)) -- 10
```
---
***
___
## API Reference
### Constants
| Constant | Description | Value |
