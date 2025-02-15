---
title: Color
nav_order: 251
parent: Generic Presets
layout: component
component_name: Color Preset
since_version: 0.2.0
---

Sets a given local or synchronized value to the given preset when `_Apply()` is invoked.

## Parameters

| Parameter Name          | Default Value | Description                                                         |
|-------------------------|---------------|---------------------------------------------------------------------|
| Use synchronized target | False         | Selects whether a local or synchronized Color should be written to. |
| Local target            | None          | Color value to write to.                                            |
| Synchronized target     | None          | Color value to write to.                                            |
| Preset                  | (0, 0, 0, 1)  | Preset value.                                                       |

## Functions

| Function Name | Description         |
|---------------|---------------------|
| _Apply        | Applies the preset. |