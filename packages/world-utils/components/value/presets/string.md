---
title: String
nav_order: 254
parent: Generic Presets
layout: component
component_name: String Preset
since_version: 0.2.0
---

Sets a given local or synchronized value to the given preset when `_Apply()` is invoked.

## Parameters

| Parameter Name          | Default Value | Description                                                          |
|-------------------------|---------------|----------------------------------------------------------------------|
| Use synchronized target | False         | Selects whether a local or synchronized String should be written to. |
| Local target            | None          | String value to write to.                                            |
| Synchronized target     | None          | String value to write to.                                            |
| Preset                  | ""            | Preset value.                                                        |

## Functions

| Function Name | Description         |
|---------------|---------------------|
| _Apply        | Applies the preset. |