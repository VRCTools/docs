---
title: Int
nav_order: 253
parent: Generic Presets
layout: component
component_name: Int Preset
since_version: 0.2.0
---

Sets a given local or synchronized value to the given preset when `_Apply()` is invoked.

## Parameters

| Parameter Name      | Default Value | Description                        |
|---------------------|---------------|------------------------------------|
| Target              | LOCAL         | Value to which to write the state. |
| Local target        | None          | Int value to write to.             |
| Synchronized target | None          | Int value to write to.             |
| Preset              | 0             | Preset value.                      |

## Functions

| Function Name | Description         |
|---------------|---------------------|
| _Apply        | Applies the preset. |