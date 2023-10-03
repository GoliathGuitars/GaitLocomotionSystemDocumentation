## Gait Locomotion Camera Animation Instance
>
> 1. Create Animation Blueprint.
>> ![](/Assets/Images/Documentation/Camera/GaitCameraAnimInstance/CreateAnimationBlueprint.png#small-image)
>
> 2. Show Plugin and Engine Content if Camera Skeleton is not an option.
>> ![](/Assets/Images/Documentation/Camera/GaitCameraAnimInstance/ShowPluginContent.png#small-image)
>
> 3. Select Camera Skeleton, and GaitCameraAnimInstance as Parent Class.
>> ![](/Assets/Images/Documentation/Camera/GaitCameraAnimInstance/CameraSkeleAndInstanceType.png#small-image)
>
> 4. Add Bpi_CameraInterface.
>> ![](/Assets/Images/Documentation/Camera/GaitCameraAnimInstance/AddInterface.png#small-image)
>
> 5. Override Interface Function, Create Data Asset Variable, and Set to Default (If no Data Asset has been created see [GaitLoco_CameraData]() and return to this step after.
>> ![](/Assets/Images/Documentation/Camera/GaitCameraAnimInstance/OverrideAndSet.png#small-image)
>
> 6. In the Anim Graph, Get Camera Data.
>> ![](/Assets/Images/Documentation/Camera/GaitCameraAnimInstance/GetData.png#small-image)
>
> 7. Split Struct Pin for State Variable.
>> ![](/Assets/Images/Documentation/Camera/GaitCameraAnimInstance/BreakStruct.png#small-image)
>
> 8. Add Modify Curve Node, and Add Curve Pins as Required.
>> ![](/Assets/Images/Documentation/Camera/GaitCameraAnimInstance/ModifyCurve.png#small-image)
>
> 9. Construct Anim Graph as Required. Thread Safe Variables can be accessed from the Main Anim Instance.
>> ![](/Assets/Images/Documentation/Camera/GaitCameraAnimInstance/AnimGraphLayout.png#small-image)
