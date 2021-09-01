# Interior Modifier Subset

![](../../.gitbook/assets/Interior_Modifier_Subset.png)

![](../../.gitbook/assets/Interior_Modifier_Subset%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Interior%20Modifier%20Subset.py)

Create a list of interior modifiers that can be used to edit or create a ModifierSet object.

## Inputs

* **interior\_wall**

  A modifier object for interior walls \(or text for the identifier of the modifier within the library\). 

* **ceiling**

  A modifier object for ceilings \(or text for the identifier of the modifier within the library\). 

* **interior\_floor**

  A modifier object for interior floors \(or text for the identifier of the modifier within the library\). 

* **interior\_window**

  A modifier object for all apertures with a Surface boundary condition. This can also be text for the identifier of the modifier within the library. 

* **interior\_door**

  A modifier object for all opaque doors with a Surface boundary condition. This can also be text for the identifier of the modifier within the library. 

* **int\_glass\_door**

  A modifier object for all glass doors with a Surface boundary condition. This can also be text for the identifier of the modifier within the library. 

## Outputs

* **interior\_set**

  A list of interior modifiers that can be used to edit or create a ModifierSet object. 

