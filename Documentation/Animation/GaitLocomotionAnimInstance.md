## Gait Locomotion Animation Instance
>
#### This is the Main Anim Instance for Gait Locomotion, Unless you Opt for the [GaitLocoGasAnimInstance](https://github.com/GoliathGuitars/GaitLocomotionSystem/blob/main/Documentation/Animation/GaitLocoGasAnimInstance.md), which is simply a child of this class, with GAS Property Mapping.
>
> - **This Class exists to house the state machine, and provide thread safe variables for common animation functions**
>> - **Animation Layer Interface Nodes are then used in these states and linked via Animation Layer Interface to the** [GaitLocomotionLayerAnimInstance](https://github.com/GoliathGuitars/GaitLocomotionSystem/blob/main/Documentation/Animation/GaitLocomotionLayerAnimInstance.md)
>>> - **Child Blueprints of [GaitLocomotionLayerAnimInstance](https://github.com/GoliathGuitars/GaitLocomotionSystem/blob/main/Documentation/Animation/GaitLocomotionLayerAnimInstance.md) are then used to reference Animation Sequences, and the Layers are finally linked via Function from a mesh reference.**
---
> - Thread Safe Variables can be found here.
>> ![](/Assets/Images/Documentation/Animation/GaitLocomotionAnimInstance/Variables.png#small-image)
---
> - Descriptions are provided so you can use them in your own thread safe functions.
>> ![](/Assets/Images/Documentation/Animation/GaitLocomotionAnimInstance/VariableDescriptions.png#small-image)
---
> - Functions are also available under "GaitLoco".
>> ![](/Assets/Images/Documentation/Animation/GaitLocomotionAnimInstance/Functions.png#small-image)
---
> - Anim Node Functions are available, and should only be called within Anim Node Functions (Marked Thread Safe)
>> ![](/Assets/Images/Documentation/Animation/GaitLocomotionAnimInstance/AnimNodeFunctions.png#small-image)
---
> - Where to create and assign anim nodes. Call the appropriate functions within these (I recommend naming them similar to avoid confusion later).
>> ![](/Assets/Images/Documentation/Animation/GaitLocomotionAnimInstance/AnimNodeExample.png#small-image)
