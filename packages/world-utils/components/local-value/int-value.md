---
title: Local Int
layout: component
nav_order: 243
parent: Local Values
component_name: Local Int Value
since_version: 0.1.0
---

Provides a local int value which may be used for changing material appearances.

## Parameters

| Parameter Name | Default Value | Description                                                      |
|----------------|---------------|------------------------------------------------------------------|
| Default Value  | 0             | The value with which this value is initialized.                  |
| Restrict Value | False         | Whether the value will be clamped between a minimum and maximum. |
| Minimum Value  | 0             | Minimum to which this value is clamped.                          |
| Maximum Value  | 1             | Maximum to which this value is clamped.                          |

## Events

| Event Name    | Description                                   |
|---------------|-----------------------------------------------|
| STATE_UPDATED | Emitted when internal value has been changed. |