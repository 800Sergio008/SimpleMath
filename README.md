# SimpleMath

## Description
A pure Luau implementation of mathematical functions, constants, and utilities built without reliance on Roblox's native `math` library. Written with strict dynamic typing `--!strict` and high precision approximations.

## Capabilities
- Strict Type Checking: built with `--!strict` mode for robust integration
- Zero External Dependencies: implements algorithms (Taylor series, Newton-Raphson, Polynomial Approximations) from scratch
- Comprehensive API: standard math operations, logarithmic and exponential calculations, trigonometry, and range utilities
- Immutable: prevented runtime mutation

---
***
___
## Installation
1. Copy the contents of `SimpleMath.luau` into a ModuleScript inside your Roblox project or Luau application
2. Require the module whenever needed:
```luau
local SimpleMath = require(path.to.SimpleMath)
```
