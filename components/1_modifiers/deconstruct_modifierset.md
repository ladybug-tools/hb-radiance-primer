# Deconstruct ModifierSet

![](../../.gitbook/assets/Deconstruct_ModifierSet.png)

![](../../.gitbook/assets/Deconstruct_ModifierSet%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Deconstruct%20ModifierSet.py)

Deconstruct a modifier set into its constituient exterior modifiers.

## Inputs

* **mod\_set \[Required\]**

  A modifier set to be deconstructed. This can also be text for a modifier set to be looked up in the modifier set library. 

## Outputs

* **exterior\_wall**

  A modifier object for the set's exterior walls. 

* **exterior\_roof**

  A modifier object for the set's exterior roofs. 

* **exposed\_floor**

  A modifier object for the set's exposed floors. 

* **window**

  A modifier object for apertures with an Outdoors boundary condition and a Wall face type for their parent face. 

* **skylight**

  A modifier object for apertures with an Outdoors boundary condition and a RoofCeiling or Floor face type for their parent face. 

* **operable**

  A modifier object for apertures with an Outdoors boundary condition and True is\_operable property. 

* **exterior\_door**

  A modifier object for opaque doors with an Outdoors boundary condition and a Wall face type for their parent face. 

* **overhead\_door**

  A modifier object for opaque doors with an Outdoors boundary condition and a RoofCeiling or Floor face type for their parent face. 

* **glass\_door**

  A modifier object for all glass doors with an Outdoors boundary condition. 

* **exterior\_shade**

  A modifier object for all exterior shades. 

