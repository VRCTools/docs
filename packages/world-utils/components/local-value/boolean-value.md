---
title: Local Boolean
layout: component
nav_order: 240
parent: Local Values
component_name: Local Boolean Value
since_version: 0.1.0
---

Provides a local on/off value which may be used for en-/disabling objects, swapping materials or changing
material appearance.

## Parameters

| Parameter Name | Default Value | Description                                             |
|----------------|---------------|---------------------------------------------------------|
| Default Value  | False         | Defines the value with which this value is initialized. |

## Events

| Event Name    | Description                                   |
|---------------|-----------------------------------------------|
| STATE_UPDATED | Emitted when internal value has been changed. |

## Functions

| Function Name | Description                                                             |
|---------------|-------------------------------------------------------------------------|
| _SetTrue()    | Sets the current state to True                                          |
| _SetFalse()   | Sets the current state to False                                         |
| _Toggle()     | Inverts the current state (e.g. False becomes True, True becomes False) |