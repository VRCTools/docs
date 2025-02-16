---
title: Boolean Operation
nav_order: 250
parent: Generic Converters
layout: component
component_name: Boolean Operation Converter
since_version: 0.3.0
---

Performs boolean operations on one or two boolean values and writes the result to a given target.

## Operations

| Operation | Formula     |
|-----------|-------------|
| NOT       | `!A`        |
| AND       | `A & B`     |
| OR        | `A | B`     |
| XOR       | `A  ^ B`    |
| NAND      | `!(A & B)`  |
| NOR       | `!(A | B)`  |
| XNOR      | `!(A ^ B)`  |

## Parameters

| Parameter Name          | Default Value | Description                        |
|-------------------------|---------------|------------------------------------|
| Target                  | LOCAL         | Value to which to write the state. |
| Local target            | None          | Boolean value to write to.         |
| Synchronized target     | None          | Boolean value to write to.         |
| Operation               | NOT           | Operation to execute.              |
| Source (A)              | LOCAL         | Source to pull from.               |
| Local Source (A)        | None          | First boolean value to read from.  |
| Synchronized Source (A) | None          | First boolean value to read from.  |
| Source (B)              | LOCAL         | Source to pull from.               |
| Local Source (B)        | None          | Second boolean value to read from. |
| Synchronized Source (B) | None          | Second boolean value to read from. |