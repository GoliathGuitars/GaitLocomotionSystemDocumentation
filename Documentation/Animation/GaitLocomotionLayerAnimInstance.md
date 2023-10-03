## Gait Locomotion Layer Animation Instance
>
#### This is the Layer Anim Instance for Gait Locomotion. This is used primarily to be the parent of child blueprints, in which Animation Sequences are set.
>
> - This Class exists to support the [GaitLocomotionAnimInstance](https://github.com/GoliathGuitars/GaitLocomotionSystem/blob/main/Documentation/Animation/GaitLocomotionAnimInstance.md) class, using a Animation Layer Interface to set Animation Sequences, when layers are linked.
>> - Animation Layer Functions are Overriden in this class, and On Relevant/Update Logic should be placed within each state see [ExampleProject]() or [ExampleTutorial]().
>>> - Child Blueprints of GaitLocomotionLayerAnimInstance are then created, Animation Sequences are set, and these layer classes are linked via mesh component.
>
> - Thread Safe Layer Variables with Descriptions. Main Anim Instance Variables are also available via PropertyAccess (Thread Safe).
>> ![](/Assets/Images/Documentation/Animation/GaitLocomotionLayerAnimInstance/Variables.png#small-image)
>
> - Layer Functions, most of the functions in this blueprint are AnimNodeFunctions (See below)
>> ![](/Assets/Images/Documentation/Animation/GaitLocomotionLayerAnimInstance/Functions.png#small-image)
>
> - Layer Anim Node Functions, must be used within Anim Node Functions, marked thread safe. (I recommend using similar names for functions to avoid confusion later).
>> ![](/Assets/Images/Documentation/Animation/GaitLocomotionLayerAnimInstance/AnimNodeFunctions.png#small-image)
