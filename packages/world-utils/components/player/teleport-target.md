---
title: Teleport Target
layout: component
nav_order: 240
parent: Player
component_name: Player Teleport Target
since_version: 0.2.0
---

Teleports players to a given target location.

## Parameters

| Parameter Name | Default Value | Description                                                                                                                     |
|----------------|---------------|---------------------------------------------------------------------------------------------------------------------------------|
| Target         | None          | Defines the location to which this component will teleport players (if null the parent object's location and rotation is used). |

## Events

| Event Name    | Description                                                 |
|---------------|-------------------------------------------------------------|
| TELEPORTED_TO | Emitted when the local player is teleported to this target. |

## Functions

| Function Name | Description                                |
|---------------|--------------------------------------------|
| _TeleportTo() | Teleports the local player to this target. |