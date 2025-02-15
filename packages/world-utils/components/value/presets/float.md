---
title: Float
nav_order: 252
parent: Generic Presets
layout: component
component_name: Float Preset
since_version: 0.2.0
---

Sets a given local or synchronized value to the given preset when `_Apply()` is invoked.

## Parameters

| Parameter Name          | Default Value | Description                                                         |
|-------------------------|---------------|---------------------------------------------------------------------|
| Use synchronized target | False         | Selects whether a local or synchronized float should be written to. |
| Local target            | None          | Float value to write to.                                            |
| Synchronized target     | None          | Float value to write to.                                            |
| Preset                  | 0.0           | Preset value.                                                       |

## Functions

| Function Name | Description         |
|---------------|---------------------|
| _Apply        | Applies the preset. |