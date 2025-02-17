---
title: Material Property
nav_order: 251
parent: Local Applicators
layout: component
component_name: Local Material Property Applicator
since_version: 0.1.0
---

Applies the state of a selection of local values to a given renderer (as a material property block) or material asset.

## Parameters

| Parameter Name     | Default Value | Description                                                              |
|--------------------|---------------|--------------------------------------------------------------------------|
| Target             | MATERIAL      | Select material, property block or global as target.                     |
| Renderer           | None          | Renderer to apply properties to (only if Use Property Block is enabled)  |
| Material           | None          | Material to apply properties to (only if Use Property Block is disabled) |
| Boolean Properties |               | Mapping of boolean values to parameter names.                            |
| Color Properties   |               | Mapping of color values to parameter names.                              |
| Float Properties   |               | Mapping of float values to parameter names.                              |
| Int Properties     |               | Mapping of int values to parameter names.                                |
| Vector3 Properties |               | Mapping of Vector3 values to parameter names.                            |

## Usage

### Property Block

If the target material's shader supports instancing and the target renderer is using only a single material (or
changing all materials is desired), you may use this mode. Changes made to the renderer **will not affect** other
objects using the same material. Ensure that `Enable Instancing` has been selected within the Material properties.
Note that most standard and common world shaders support instancing out of the box. More niche effect shaders (e.g.
caustics, water, fake lighting) may not always support instancing. Always verify that your shaders have been written
with instancing in mind.

1. Ensure the target materials have "Enable Instancing" ticked
2. Tick "Use Property Block"
3. Drag the target renderer into the "Renderer" field
4. Create a separate entry for each parameter you'd like to drive using the target parameter name.

**Important:** Parameter names typically do not match the displayed names. See below.

### Material

1. Ensure "Use Property Block" is not ticked
2. Drag the target material into the "Material" field
3. Create a separate entry for each parameter you'd like to drive using the target parameter name.

**Important:** Changes made to the material **will affect all renderers using the same material**. Additionally,
changes in play mode may be retained on the material after exiting play mode.

**Important:** Parameter names typically do not match the displayed names. See below.

### Finding Parameter Names

Material parameter names will practically never match the displayed names in the inspector. To get the actual names:

1. Select the maaterial in question
2. Right click on the preview on the top - left of the material name
3. Select "Select Shader"
4. All parameters will be displayed with their actual names within the inspector window

Note that some shaders are provided with custom inspector implementations which may mask complexity in the shader
parameters. If it isn't clear which parameters to select, contact the shader author.

### Common Parameter Names

These parameter name mappings are commonly used but may differ from implementation to implementation. Only use them
as a rough guide.

| Displayed Name | Actual Name      |
|----------------|------------------|
| Alpha Cutoff   | `_Cutoff`        |
| Color          | `_Color`         |
| Emission Color | `_EmissionColor` |
| Metallic       | `_Metallic`      |
| Smoothness     | `_Glossiness`    |
| Roughness      | `_Roughness`     |