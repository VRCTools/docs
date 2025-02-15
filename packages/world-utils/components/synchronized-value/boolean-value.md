---
title: Synchronized Boolean
layout: component
nav_order: 240
parent: Synchronized Values
since_version: 0.1.0
component_name: Synchronized Boolean Value
networked: true
---

Provides a synchronized on/off value which may be used for en-/disabling objects, swapping materials or changing
material appearance.

## Parameters

| Parameter Name | Default Value | Description                                             |
|----------------|---------------|---------------------------------------------------------|
| Default Value  | False         | Defines the value with which this value is initialized. |

## Events

| Event Name    | Description                                   |
|---------------|-----------------------------------------------|
| STATE_UPDATED | Emitted when internal value has been changed. |