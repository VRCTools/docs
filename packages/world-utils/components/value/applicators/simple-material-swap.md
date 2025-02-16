---
title: Simple Material Swap
nav_order: 253
parent: Generic Applicators
layout: component
component_name: Simple Material Swap Applicator
since_version: 0.1.0
---

Replaces the material of one or more objects based on the value of a local boolean.

## Parameters

| Parameter Name     | Default Value | Description                                                                                     |
|--------------------|---------------|-------------------------------------------------------------------------------------------------|
| Source             | LOCAL         | Value from which to pull the state.                                                             |
| Local Value        | None          | Value from which to pull the state.                                                             |
| Synchronized value | None          | Value from which to pull the object state.                                                      |
| Swaps              |               | Mapping of renderer, material slot and replacement material.                                    |
| Invert             | False         | Invert the behavior relative to the local value (e.g. off means replacement, on means regular). |