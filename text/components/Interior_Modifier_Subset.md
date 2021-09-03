## Interior Modifier Subset

![](../../images/components/Interior_Modifier_Subset.png)

![](../../images/icons/Interior_Modifier_Subset.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Interior%20Modifier%20Subset.py)


Create a list of interior modifiers that can be used to edit or create a ModifierSet object. 



#### Inputs
* ##### interior_wall 
A modifier object for interior walls (or text for the identifier of the modifier within the library). 
* ##### ceiling 
A modifier object for ceilings (or text for the identifier of the modifier within the library). 
* ##### interior_floor 
A modifier object for interior floors (or text for the identifier of the modifier within the library). 
* ##### interior_window 
A modifier object for all apertures with a Surface boundary condition. This can also be text for the identifier of the modifier within the library. 
* ##### interior_door 
A modifier object for all opaque doors with a Surface boundary condition. This can also be text for the identifier of the modifier within the library. 
* ##### int_glass_door 
A modifier object for all glass doors with a Surface boundary condition. This can also be text for the identifier of the modifier within the library. 

#### Outputs
* ##### interior_set
A list of interior modifiers that can be used to edit or create a ModifierSet object. 