---
title: Float Label
nav_order: 262
parent: Local UI
layout: component
component_name: Local Float Label
since_version: 0.1.0
---

Displays the current value of a local float.

## Parameters

| Parameter Name | Default Value | Description                                                   |
|----------------|---------------|---------------------------------------------------------------|
| Local Value    | None          | Value from which to pull the object state.                    |
| Enable Mapping | False         | En-/Disables mapping of the float value for display purposes. |
| Range          | 0, 100        | Range to which the value will be mapped.                      |
| Multiplier     | 100           | Multiplier with which the value will be multiplied.           |

The order of operations for mappings is `Range -> Multiplier` meaning the formula for displaying values will be
`remap(value) * multiplier`

**Important:** `Enable Mapping` requires the referenced float to be restricted in order to work.

## Usage

Attach this component to an object which also contains a Text Mesh Pro UGUI component. The label will make use of the
text present within the Text Mesh component and will be formatted using [C#'s string.format][string-format] using only
a single argument.

For example, to display the value as-is, `{0}` may be used. To prefix the value you may also write `Percentage: {0}`.
Additionally, you may adjust the way numbers are formatted. For instance, you may change the number of digits displayed
as follows: `{0:000}` resulting in the number being displayed as three digits at all times. A percentage, may be
formatted as `Brightness: {0:000}%`, for instance.

[string-format]: https://learn.microsoft.com/en-us/dotnet/fundamentals/runtime-libraries/system-string-format