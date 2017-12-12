# mun-three-utils

This is a collection of utilitites we use at MUN when working with three.js. Many of them are adapted from [Jack Rugile](https://github.com/jackrugile).

## Installation
`npm install --save mun-three-utils`

ES6

`import * as THREEUTILS from 'mun-three-utils`

ES5

`var THREEUTILS = require(mun-three-utils)`

# Calc
This utility provides commonly used calculations for three.js.

- [rand](#randmin-max-ease)
- [randInt](#randint-min-max-ease)

## `rand(min, max, ease)`
Returns a random float between two values, with the option of easing bias.

| Parameter | Type | Description |
|:---|:---|:---|
| min | `Number` | The minimum float value. |
| max | `Number` | The maximum float value. |
| ease | `Function` | Easing function to apply to the random value |

## `randInt(min, max, ease)`
Returns a random integer between two values, with the option of easing bias.

| Parameter | Type | Description |
|:---|:---|:---|
| min | `Number` | The minimum integer value. |
| max | `Number` | The maximum integer value. |
| ease | `Function` | Easing function to apply to the random value |

## `randArr(arr)`
Returns a random item from an array.

| Parameter | Type | Description |
|:---|:---|:---|
| arr | `Array` | The array to randomly pull from. |

## `map(val, inputMin, inputMax, outputMin, outputMax)`
Returns a mapped value from and input min/max to an output min/max.

| Parameter | Type | Description |
|:---|:---|:---|
| val | `Number` | Input value. |
| inputMin | `Number` | Minimum of input range. |
| inputMax | `Number` | Maximum of input range. |
| outputMin | `Number` | Minimum of output range. |
| outputMax | `Number` | Maximum of output range. |

## `clamp(val, min, max)`
Restricts a value to a min/max range.

| Parameter | Type | Description |
|:---|:---|:---|
| val | `Number` | Value to be clamped. |
| min | `Number` | Minimum of clamped range. |
| max | `Number` | Maximum of clamped range. |

## `lerp(current, target, mix)`
Linearly interpolates between two vectors.

| Parameter | Type | Description |
|:---|:---|:---|
| current | `Number` | Current position. |
| target | `Number` | Target position. |
| mix | `Number` | Speed of the interpolation. |

## `roundToUpperInterval(value, interval)`
Round up a value to the next highest interval.

| Parameter | Type | Description |
|:---|:---|:---|
| value | `Number` | Value to be rounded. |
| interval | `Number` | Interval. |

## `roundToLowerInterval(value, interval)`
Round down a value to the next lowest interval.

| Parameter | Type | Description |
|:---|:---|:---|
| value | `Number` | Value to be rounded. |
| interval | `Number` | Interval. |

## `roundToNearestInterval(value, interval)`
Round a value to the nearest interval.

| Parameter | Type | Description |
|:---|:---|:---|
| value | `Number` | Value to be rounded. |
| interval | `Number` | Interval. |

## `intersectSphere(a, b)`
Check if two sphere are intersecting in 3D space.

| Parameter | Type | Description |
|:---|:---|:---|
| a | `Object` | Sphere 1 with radius, x, y, and z. |
| b | `Object` | Sphere 2 with radius, x, y, and z. |

## `getIndexFromCoords(x, y, w)`
Convert from grid coords to index.

| Parameter | Type | Description |
|:---|:---|:---|
| x | `Number` | X value (column). |
| y | `Number` | Y value (row). |
| x | `Number` | Width of grid. |

## `getCoordsFromIndex(i, w)`
Convert from index to grid coords.

| Parameter | Type | Description |
|:---|:---|:---|
| i | `Number` | Index. |
| w | `Number` | Width of grid. |

## `visibleHeightAtZDepth(depth, camera)`
Returns the visible height in your scene at a given distance from a PerspectiveCamera.

| Parameter | Type | Description |
|:---|:---|:---|
| depth | `Number` | Depth of current plane. |
| camera | `Object` | PerspectiveCamera object. |

## `visibleWidthAtZDepth(depth, camera)`
Returns the visible width in your scene at a given distance from a PerspectiveCamera.

| Parameter | Type | Description |
|:---|:---|:---|
| depth | `Number` | Depth of current plane. |
| camera | `Object` | PerspectiveCamera object. |

# Ease

A collection of commonly used easing functions.

## `inQuad(t, b, c, d)`
Returns an eased float value based on inQuad.

| Parameter | Type | Description |
|:---|:---|:---|
| t | `Number` | Current time. |
| b | `Number` | Begining time. |
| c | `Number` | Change in value. |
| d | `Number` | Duration. |

## `outQuad(t, b, c, d)`
Returns an eased float value based on outQuad.

| Parameter | Type | Description |
|:---|:---|:---|
| t | `Number` | Current time. |
| b | `Number` | Begining time. |
| c | `Number` | Change in value. |
| d | `Number` | Duration. |


## `inOutQuad(t, b, c, d)`
Returns an eased float value based on inOutQuad.

| Parameter | Type | Description |
|:---|:---|:---|
| t | `Number` | Current time. |
| b | `Number` | Begining time. |
| c | `Number` | Change in value. |
| d | `Number` | Duration. |


## `inCubic(t, b, c, d)`
Returns an eased float value based on inCubic.

| Parameter | Type | Description |
|:---|:---|:---|
| t | `Number` | Current time. |
| b | `Number` | Begining time. |
| c | `Number` | Change in value. |
| d | `Number` | Duration. |


## `outCubic(t, b, c, d)`
Returns an eased float value based on outCubic.

| Parameter | Type | Description |
|:---|:---|:---|
| t | `Number` | Current time. |
| b | `Number` | Begining time. |
| c | `Number` | Change in value. |
| d | `Number` | Duration. |


## `inOutCubic(t, b, c, d)`
Returns an eased float value based on inOutCubic.

| Parameter | Type | Description |
|:---|:---|:---|
| t | `Number` | Current time. |
| b | `Number` | Begining time. |
| c | `Number` | Change in value. |
| d | `Number` | Duration. |
