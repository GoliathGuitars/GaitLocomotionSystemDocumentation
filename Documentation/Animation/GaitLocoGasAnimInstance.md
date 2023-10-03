## Gait Locomotion GAS Animation Instance
>
#### This is an optional child class of [GaitLocomotionAnimInstance](https://github.com/GoliathGuitars/GaitLocomotionSystem/blob/main/Documentation/Animation/GaitLocomotionAnimInstance.md) to add GAS Property Mapping, allowing for significantly easier state management with Gameplay Abilities.
>
> 1. Within your Gameplay Ability Class you will create your tag, if your Ability System Component has this tag, the boolean in the Anim Instance Property Mapping will be true.
>> ![](/Assets/Images/Documentation/Animation/GaitLocoGasAnimInstance/PropertyTags.png#small-image)
---
> 2. Although technically optional, for [GaitCameraAnimInstance](https://github.com/GoliathGuitars/GaitLocomotionSystem/blob/main/Documentation/Camera/GaitCameraAnimInstance.md) to return true for some variables (Crouch/Sprint/IsRightShoulder), it is necessary to override the Blueprint Thread Safe Update Animation Function.
>> ![](/Assets/Images/Documentation/Animation/GaitLocoGasAnimInstance/ThreadSafeOverride.png#small-image)
---
> 3. After that create your property mapping using ability tags, and create booleans to match. Then set the "GaitLocomotion" Variables from those using the Blueprint Thread Safe Update Animation.
>> - This unfortunate workaround is due to the fact that you cannot set variables that exist in C++ like IsRightShoulder in Property Mapping, which are necessary for calculations (RootYawOffset). Also due to that means the Camera, which reads properties at a C++ level, cannot perform those transitions without them being set in blueprint as shown.
>>> - Ultimately I settled on this solution as to remain agnostic in design and not force anyone to use GAS, or set those variables in any particular way. You could set them with an interface message, which is a pretty standard non GAS way of activating booleans within an Anim Instance.
>>>> ![](/Assets/Images/Documentation/Animation/GaitLocoGasAnimInstance/PropertyMapping.png#small-image)
