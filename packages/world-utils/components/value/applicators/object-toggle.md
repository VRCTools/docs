---
title: Object Toggle
nav_order: 250
parent: Generic Applicators
layout: component
component_name: Object Toggle Applicator
since_version: 0.1.0
---

En-/Disables one or more objects based on the state of a local boolean.

## Parameters

| Parameter Name     | Default Value | Description                                                                                 |
|--------------------|---------------|---------------------------------------------------------------------------------------------|
| Source             | LOCAL         | Value from which to pull the state.                                                         |
| Local Value        | None          | Value from which to pull the object state.                                                  |
| Synchronized value | None          | Value from which to pull the object state.                                                  |
| Targets            |               | List of objects to update.                                                                  |
| Invert             | False         | Invert the behavior relative to the local value (e.g. off means active, on means disabled). |