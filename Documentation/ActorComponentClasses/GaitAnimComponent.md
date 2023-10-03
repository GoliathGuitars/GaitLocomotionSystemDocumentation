## Gait Locomotion Animation Component

#### This class may get completely deprecated over time as more ideal solutions are found.
>
> 1. Add GaitAnim Component to your actor, and Set Rotation Type and Aim Solver Data if Required (***IsFirstPerson will only change the trace position to camera center for AimSolver for now***)
>> ![](/Assets/Images/Documentation/ActorComponentClasses/GaitAnimComponent/GaitLocoComponentClassDefaults.png#small-image)
>
> 2. Aim Solver Property Access Variables will now function within the animation graph.
>> ![](/Assets/Images/Documentation/ActorComponentClasses/GaitAnimComponent/AimSolverPropertyAccess.png#small-image)
>>> - It is recommended to use the Aim Solver Transform with [DragonIK](https://www.unrealengine.com/marketplace/en-US/product/dragon-ik-animal-inverse-kinematics) Aim Solver Node as a simple thread safe upper body Aim Solver Solution.
