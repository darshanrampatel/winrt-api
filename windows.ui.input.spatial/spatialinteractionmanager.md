---
-api-id: T:Windows.UI.Input.Spatial.SpatialInteractionManager
-api-type: winrt class
---

<!-- Class syntax.
public class SpatialInteractionManager : Windows.UI.Input.Spatial.ISpatialInteractionManager
-->

# Windows.UI.Input.Spatial.SpatialInteractionManager

## -description
Provides access to user input from hands, controllers, and system voice commands.

## -remarks
Spatial gestures are a key form of input for HoloLens. By routing the interactions from the SpatialInteractionManager to a hologram's SpatialGestureRecognizer, apps can detect Tap, Hold, Manipulation, and Navigation events uniformly across hands, voice and controllers.

Interactions are mostly opaque, with an event triggering only at the beginning, so the gesture recognizer you route it to can capture the interaction in its entirety. Apps can instead choose to use the low-level Source events or poll using GetDetectedSourcesAtTimestamp to manually process the Presses, Updates, and Releases surfaced by a given hand or controller.

## -examples

## -see-also
