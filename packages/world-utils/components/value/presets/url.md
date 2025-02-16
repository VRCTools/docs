---
title: URL
nav_order: 255
parent: Generic Presets
layout: component
component_name: URL Preset
since_version: 0.2.0
---

Sets a given local or synchronized value to the given preset when `_Apply()` is invoked.

## Parameters

| Parameter Name      | Default Value | Description                        |
|---------------------|---------------|------------------------------------|
| Target              | LOCAL         | Value to which to write the state. |
| Local target        | None          | URL value to write to.             |
| Synchronized target | None          | URL value to write to.             |
| Preset              | ""            | Preset value.                      |

## Functions

| Function Name | Description         |
|---------------|---------------------|
| _Apply        | Applies the preset. |