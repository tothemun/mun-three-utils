# mun-three-utils

This is a collection of utilitites we use at MUN when working with three.js. Many of them are adapted from [Jack Rugile](https://github.com/jackrugile).

## Installation
`npm install --save mun-three-utils`

ES6
`import * as THREEUTILS from 'mun-three-utils`

ES5
`var THREEUTILS = require(mun-three-utils)`

# Utilities

## Calc
This utility provides commonly used calculations for three.js.

## `rand(min, max, ease)`
Returns a random float.

| Parameter | Type | Description |
|:---|:---|:---|
| min | `Float` | The minimum float value. |
| max | `Float` | The maximum float value. |
| ease | `Function` | Easing function to apply to the random value |
