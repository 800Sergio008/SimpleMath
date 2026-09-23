> VERSION: 1.0.0

# SimpleMath

## Description
A pure Luau implementation of mathematical functions, constants, and utilities built without reliance on Roblox's native `math` library. Written with strict dynamic typing `--!strict` and high precision approximations.

## Capabilities
- Strict Type Checking: built with `--!strict` mode for robust integration.
- Zero External Dependencies: implements algorithms (Taylor series, Newton-Raphson, Polynomial Approximations) from scratch.
- Comprehensive API: standard math operations, logarithmic and exponential calculations, trigonometry, and range utilities.
- Immutable: prevented runtime mutation.

---
---
## Installation
1. Copy the contents of `SimpleMath.luau` into a ModuleScript inside your Roblox project or Luau application.
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
---
## API Reference
### Constants
| Constant | Description | Value |
| -------- | ----------- | ----- |
| MIN_VALUE | Minimum positive floating point number | 5e-324 |
| MAX_VALUE | Maximum positive floating point number | 1.79e+308 |
| E | Euler's constant (*e*) | 2.7182818284590452354 |
| LOG2E | Base-2 logarithm of *e* | 1.4426950408889634074 |
| LOG10E | Base-10 logarithm of *e* | 0.43429448190325182765 |
| LN2 | Natural logarithm of 2 | 0.69314718055994530942 |
| LN10 | Natura logarithm of 10 | 2.30258509299404568402 |
| SQRT2 | Square root of 2 | 1.41421356237309504880 |
| SQRT1_2 | Square root of 1/2 | 0.70710678118654752440 |
| PI | Archimedes' constants (*π*) | 3.14159265358979323846 |
| TAU | 2 ⅹ π | 6.28318530718 | 6.2831853071795864769 |
| EPSILON | Machine precision threshold | 1e-6 |
| HUGE | Representation of positive infinity (∞) | 1/0 |
| NAN | Representation of Not-a-Number | 0/0 |
| DEG2RAD | Multiplier to convert degrees to radians | π/180 |
| RAD2DEG | Multiplier to convert radians to degrees | 180/π |

### Math Functions
| Method | Parameter(*s*) | Value |
| ------ | -------------- | ----- |
| Math.Fabs | number | number |
| Math.Floor | number | number |
| Math.Ceil | number | number |
| Math.Round | number, number? | number |
| Math.Trunc | number | number |
| Math.Fmod | number, number | number |
| Math.Modf | number | number, number |
### Power and Logarithmic Functions
| Method | Parameter(*s*) | Value |
| ------ | -------------- | ----- |
| Math.Exp | number | number |
| Math.Log | number | number |
| Math.Log10 | number | number |
| Math.Pow | number, number | number |
| Math.Sqrt | number | number |
| Math.Frexp | number | number, number |
| Math.Ldexp | number, number | number |
### Trigonometry and Hyperbolic Functions
| Method | Parameter(*s*) | Value |
| ------ | -------------- | ----- |
| Math.Sin | number | number |
| Math.Cos | number | number |
| Math.Tan | number | number |
| Math.Atan2 | number, number | number |
| Math.Atan | number | number |
| Math.Asin | number | number |
| Math.Acos | number | number |
| Math.Sinh | number | number |
| Math.Cosh | number | number |
| Math.Tanh | number | number |
| Math.Rad | number | number |
### Advanced and Interpolation Functions
| Method | Parameter(*s*) | Value |
| ------ | -------------- | ----- |
| Math.Clamp | number, number, number | number |
| Math.Lerp | number, number, number | number |
| Math.Normalize | number, number, number | number |
| Math.Remap | number, number, number, number, number | number |
| Math.Noise | number | number |
| Math.Sign | number | number |
---
---
## License
This repository is open-source and free to use under the MIT License.
