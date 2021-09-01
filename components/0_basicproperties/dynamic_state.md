# Dynamic State

![](../../.gitbook/assets/Dynamic_State.png)

![](../../.gitbook/assets/Dynamic_State%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Dynamic%20State.py)

Create a State object representing a single dynamic group state.

## Inputs

* **modifier**

  A Honeybee Radiance Modifier object to be applied to this state's parent in this state. This is used to swap out the modifier in multi-phase studies. If None, it will be the parent's default modifier. 

* **shades**

  An optional array of StateGeometry objects to be included with this state. 

## Outputs

* **state**

  A Honeybee State object representing a single dynamic group state. This can be assigned to apertures or shades using the "HB Dynamic Aperture Group" componet or the "HB Dynamic Shade Group" component. 

