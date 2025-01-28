---
title: Slider
nav_order: 265
parent: Synchronized UI
layout: component
component_name: Synchronized Slider
since_version: 0.1.0
---

Displays and modifies the current value of a synchronized float.

## Parameters

| Parameter Name     | Default Value | Description                                         |
|--------------------|---------------|-----------------------------------------------------|
| Synchronized Value | None          | Value from which to pull the object state.          |
| Enable Mapping     | False         | En-/Disables mapping of the float value.            |
| Range              | 0, 100        | Range to which the value will be mapped.            |
| Multiplier         | 100           | Multiplier with which the value will be multiplied. |

The order of operations for mappings is `Range -> Multiplier` meaning the formula for displaying values will be
`remap(value) * multiplier`

**Important:** `Enable Mapping` requires the referenced float to be restricted in order to work.