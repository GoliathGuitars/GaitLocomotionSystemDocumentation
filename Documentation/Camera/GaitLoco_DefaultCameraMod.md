## Gait Locomotion Default Camera Modifier
#### This is details about what this class is doing, not what it can do.
> 1. Set Pivot Target from Skeletal Mesh Transform, or First Person Camera Location from Mesh Socket.
>> ![](/Assets/Images/Documentation/Camera/GaitLoco_DefaultCameraMod/SetPivotTarget.png#small-image)
>
> 2. Calculate Target Camera Rotation by interpolating Camera Rotation, to Control Rotation, using Rotation Lag Speed Curve.
>> ![](/Assets/Images/Documentation/Camera/GaitLoco_DefaultCameraMod/CalculateTargetCameraRotation.png#small-image)
>
> 3. Calculate Smoothed Pivot Target Transform by Calculating Axis without Lag. Interpolating between Smoothed Pivot Target Location, and Pivot Target Location, Target Camera Rotation and Pivot Target Rotation, using PivotLagSpeeds. 
>> ![](/Assets/Images/Documentation/Camera/GaitLoco_DefaultCameraMod/CalculateSmoothedPivotTarget.png#small-image)
>
> 4. Calculate Pivot Location by adding Smoothed Pivot Target Location, and the Vectors of Smoothed Pivot Target Rotation multiplied by PivotOffset Curve Values.
>> ![](/Assets/Images/Documentation/Camera/GaitLoco_DefaultCameraMod/CalculatePivotLocation.png#small-image)
>
> 5. Calculate Target Camera Location by adding Pivot Location, and the Vectors of Target Camera Rotation multiplied by CameraOffset Curve Values.
>> ![](/Assets/Images/Documentation/Camera/GaitLoco_DefaultCameraMod/CalculateTargetCameraLocation.png#small-image)
>
> 6. Trace for an Object between the Camera and Target, and apply Corrective Offset (***Collision Offset Functionality***)
>> ![](/Assets/Images/Documentation/Camera/GaitLoco_DefaultCameraMod/CorrectiveOffset.png#small-image)
>
> 7. Lerp Between TPP, and FPP, and Return Location/Rotation/FOV.
>> ![](/Assets/Images/Documentation/Camera/GaitLoco_DefaultCameraMod/Return.png#smallimage)
>
> - Get Curve Values from Camera Animation Instance.
>> ![](/Assets/Images/Documentation/Camera/GaitLoco_DefaultCameraMod/CameraBehaviour.png#small-image)
