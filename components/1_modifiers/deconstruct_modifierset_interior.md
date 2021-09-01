# Deconstruct ModifierSet Interior

![](../../.gitbook/assets/Deconstruct_ModifierSet_Interior.png)

![](../../.gitbook/assets/Deconstruct_ModifierSet_Interior%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Deconstruct%20ModifierSet%20Interior.py)

Deconstruct a modifier set into its constituient interior modifiers.

## Inputs

* **mod\_set \[Required\]**

  A modifier set to be deconstructed. This can also be text for a modifier set to be looked up in the modifier set library. 

## Outputs

* **interior\_wall**

  A modifier object for the set's interior walls. 

* **ceiling**

  A modifier object for the set's interior roofs. 

* **interior\_floor**

  A modifier object for the set's interior floors. 

* **interior\_window**

  A modifier object for all apertures with a Surface boundary condition. 

* **interior\_door**

  A modifier object for all opaque doors with a Surface boundary condition. 

* **int\_glass\_door**

  A modifier object for all glass doors with a Surface boundary condition. 

* **interior\_shade**

  A modifier object for all interior shades. 

