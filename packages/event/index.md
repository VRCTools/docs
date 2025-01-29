---
title: Event System
layout: package
nav_order: 200
parent: Packages
package_name: VRCTEvent
---

# Event System

The VRCTools event system provides a very simple event system for Udon# scripts letting your scripts publish or receive
updates from other components within a scene.

**Important:** This package on its own is useless. If you do not intend to write your own scripts using this library,
you likely don't need to install it yourself. Some VRCTools or third party packages may depend on it. If you are
installing via Creator Companion or an equivalent package manager, it should be installed automatically when needed.
If you are installing packages manually, refer to the documentation of the package or asset you are trying to install.

## Usage

To create an event emitter (e.g. an Udon# script which generates an arbitrary number of events which others may
listen to), you need to extend `AbstractEventEmitter` from the `VRCTools.Event` namespace:

```csharp
import VRCTools.Event;

class MyEventEmitter : AbstractEventEmitter {
   public const int EVENT_A = 0;
   public const int EVENT_B = 1;
   public const int EVENT_COUNT = 2;

   public override int EventCount => EVENT_COUNT;

   // ...

   // for instance, if you want to emit an event whenever a player enters a trigger volume
   public override void OnPlayerTriggerEnter(VRCPlayerApi player) {
      this._EmitEvent(EVENT_A);
   }
}
```

In order to subscribe to an event, you need to acquire a reference to the emitter and register yourself:

```csharp
class MyReceiver : UdonSharpBehaviour {
   public MyEventEmitter emitter;

   private void Start() {
      this.emitter._RegisterHandler(MyEventEmitter.EVENT_A, this, nameof(this._OnEventA));
   }

   // recommended to implement but technically purely optional if your object never gets destroyed
   private void OnDestroy() {
      this.emitter._UnregisterHandler(ExampleEventEmitter.EVENT_ONE, this, nameof(this._OnEvent));
      // or alternatively
      this.emitter._UnregisterHandler(this);
   }

   // Important: Handler functions have to be declared as public in order to be invoked
   public void _OnEventA() {
      // do something
   }
}
```

Please note that these are heavily simplified usage examples.
A set of full example scripts observing best practice may be found in `Packages/io.vrctools.event/Samples` (or
`Packages/VRCTools - Event System/Samples` via the Unity Editor UI).

Please also note that all event emitters are implicitly implementations of `UdonSharpBehaviour` at the moment.
This is due to limitations on the types and abstractions that Udon# can compile.