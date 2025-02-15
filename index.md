---
title: Getting Started
layout: default
nav_order: 1
---

# Getting Started

## Getting the Packages

In order to gain access to the various open source VRCTools packages, please add the public VRCTools package repository
to creator companion or an alternative package manager. The repository is currently available via `{{ site.vcc_url }}`.

You may also add the repository automatically:

[Add to VCC](vcc://vpm/addRepo?url={{ site.vcc_url | uri_escape }}){: .btn .btn-green }

Or, if this does not work:

1. Open your VCC and go to Settings
2. Click the "Packages" tab
3. Click "Add Repository"
4. In the field that appears - paste the following url: `{{ site.vcc_url }}`
5. Click "Add"
6. Check the repository info and click "I Understand"

Regardless of your method, you should now see the various VRCTools packages listed within the "Manage Project" section
of your respective world within VCC. All publicly accessible VRCTools packages may be installed, updated and removed
from there.

Please refer to the documentation of your package manager if you are using a third party tool instead of VRChat's
official creator companion.

Additionally, we offer pre-built packages for manual installation within the releases section of each library
repository on [GitHub](https://github.com/VRCtools). Please note, however, that manual installation **will not
automatically install dependencies**.

## Navigating Packages

Generally all VRCTools packages are structured in a similar fashion (with minor differences depending on their
respective purpose). All installed packages can be found within the `Packages` section of the asset browser and
will be prefixed with `VRCTools -` (for example: `VRCTools - Event System`, `VRCTools - World Utilities`).

The general directory structure will be as follows:

```
VRCTools - <package name>
 |
 +--- Editor - Custom inspectors, editor windows, context menus, etc.
 |
 +--+ Runtime - Scripts, Textures & Prefabs
 |  |
 |  +--- Materials - Materials for 3D objects, UI elements
 |  |
 |  +--- Prefabs - Example setups, basic component prefabs, etc.
 |  |
 |  +--- Textures - Textures for 3D objects, UI elements, default textures
 |  |
 |  +--- UdonScripts - Udon specific scripts (e.g. for use within VRC worlds)
 |  |
 |  +--- VRCTools.<package name>.Asmdef - C# Assembly Definition for all scripts within the library
 |
 +--- Samples - Example scenes and related resources
 |
 +--- LICENSE - Copy of the project license in full
```

Please note that the directory name on disk will be `io.vrctools.<package name>` instead of
`VRCTools - <package name>`.