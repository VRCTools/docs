---
title: Trigger Volume
layout: component
nav_order: 242
parent: Player
component_name: Player Trigger Volume
since_version: 0.2.0
---

Emits events when a player enters or leaves a given trigger volume. To be combined with a `Collider` component set to
trigger mode.

## Parameters

| Parameter Name        | Default Value | Description                                                           |
|-----------------------|---------------|-----------------------------------------------------------------------|
| Enter Events          |               | Listing of behaviours and event names to invoke when a player enters. |
| Exit Events           |               | Listing of behaviours and event names to invoke when a player leaves. |
| Accepted Player Types | None          | Filters applicable players (e.g. local/remote)                        |

## Events

| Event Name   | Description                              |
|--------------|------------------------------------------|
| PLAYER_ENTER | Emitted when a player enters the volume. |
| PLAYER_EXIT  | Emitted when a player leaves the volume. |