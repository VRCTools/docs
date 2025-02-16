---
title: String Label
nav_order: 266
parent: Generic UI
layout: component
component_name: String Label
since_version: 0.1.0
---

Displays the current value of a local string.

## Parameters

| Parameter Name     | Default Value | Description                                |
|--------------------|---------------|--------------------------------------------|
| Source             | LOCAL         | Value from which to pull the state.        |
| Local Value        | None          | Value from which to pull the object state. |
| Synchronized value | None          | Value from which to pull the object state. |

## Usage

Attach this component to an object which also contains a Text Mesh Pro UGUI component. The label will make use of the
text present within the Text Mesh component and will be formatted using [C#'s string.format][string-format] using only
a single argument.

For example, to display the value as-is, `{0}` may be used. To prefix the value you may also write `MOTD: {0}`.

[string-format]: https://learn.microsoft.com/en-us/dotnet/fundamentals/runtime-libraries/system-string-format