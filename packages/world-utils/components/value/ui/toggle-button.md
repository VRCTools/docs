---
title: Toggle Button
nav_order: 268
parent: Generic UI
layout: component
component_name: Value Toggle Button
since_version: 0.1.0
---

Toggles a local boolean value at the click of a button.

## Parameters

| Parameter Name     | Default Value   | Description                                              |
|--------------------|-----------------|----------------------------------------------------------|
| Source             | LOCAL           | Value from which to pull the state.                      |
| Local Value        | None            | Value from which to pull the object state.               |
| Synchronized value | None            | Value from which to pull the object state.               |
| Active Color       | (1, 1, 1, 1)    | Button color when toggle is active.                      |
| Inactive Color     | (.5, .5, .5, 1) | Button color when toggle is inactive.                    |
| Invert             | False           | Inverts button toggle state in reference to local value. |

## Usage

Attach this component to a standard ui Button component (TextMesh Pro variation recommended) and select the target
value.