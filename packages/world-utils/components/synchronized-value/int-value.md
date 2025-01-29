---
title: Synchronized Int
layout: component
nav_order: 243
parent: Synchronized Values
since_version: 0.1.0
component_name: Synchronized Int Value
networked: true
---

Provides a synchronized int value which may be used for changing material appearances.

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

## Functions

| Function Name | Description                 |
|---------------|-----------------------------|
| _Zero()       | Resets the value to zero    |
| _Increment()  | Increments the state by one |
| _Decrement()  | Decrements the state by one |