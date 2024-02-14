# Unity Touch Controller

## Overview
This Unity script facilitates touch-based camera and player rotation in a 3D environment. It is designed to respond to touch gestures within a specified touch panel, controlling camera movement along the X-axis and rotating the player accordingly.

## Features
- Touch-based camera and player rotation.
- Adjustable rotation speed for a customizable experience.
- X-axis rotation limits for controlled camera movement.
- Responsive touch gestures within a designated touch panel.

## Usage
1. Attach the script to a GameObject in your Unity scene.
2. Assign the necessary references such as the touch panel, player camera, and player body in the Unity Inspector.
3. Tweak parameters like `rotationSpeed` and `cameraRotationLimitX` to suit your preferences.

## Example
```csharp
// Example code snippet demonstrating how to use the touch controller script in Unity.
using UnityEngine;

public class YourExampleClass : MonoBehaviour
{
    public RectTransform yourTouchPanel;
    public Transform yourPlayerCamera;
    public Transform yourPlayerBody;

    void Start()
    {
        // Instantiate and configure the touch controller script.
        touchcontroller touchController = gameObject.AddComponent<touchcontroller>();
        touchController.touchPanel = yourTouchPanel;
        touchController.playerCamera = yourPlayerCamera;
        touchController.playerBody = yourPlayerBody;
        // Additional configuration if needed.
    }
}
