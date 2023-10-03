## Gait Locomotion Character Movement Component
>
> 1. Set Parent Character Movement Component Class to GaitLocomotionCmc.
>> ![](/Assets/Images/Documentation/ActorComponentClasses/GaitLocomotionCmc/CmcParentClass.png#small-image)
>
> 2. Call Functions as Required to Update Movement Speeds to Cmc (Replicated and Synchronized).
> - Set Movement Speed multiplier values in Class Defaults of Character Movement Component.
>> ![](/Assets/Images/Documentation/ActorComponentClasses/GaitLocomotionCmc/GaitLocoCmc.png#small-image)
>
> - This Function does not usually get called manually, but is used inside the animation graph to do predictive landing using the ground distance variable to compare to a curve.
>> ![](/Assets/Images/Documentation/ActorComponentClasses/GaitLocomotionCmc/GetGroundInfo.png#small-image)
