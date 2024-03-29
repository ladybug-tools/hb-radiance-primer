## Apply Face Modifier

![](../../images/components/Apply_Face_Modifier.png)

![](../../images/icons/Apply_Face_Modifier.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Apply%20Face%20Modifier.py)


Apply a Modifier to Honeybee Faces, Doors or Room walls. 

This component supports the assigning of different modifiers based on cardinal orientation, provided that a list of Modifiers are input to the _mod.  



#### Inputs
* ##### hb_objs [Required]
Honeybee Faces, Doors, Rooms or a Model to which the input _mod should be assigned. For the case of Rooms or a Model, the modifier will only be applied to the Room's outdoor walls. Note that, if you need to assign a modifier to all the roofs, floors, etc. of a Room, the best practice is to create a ModifierSet and assing that to the Room. 
* ##### mod [Required]
A Honeybee Modifier to be applied to the input _hb_objs. This can also be text for a modifier to be looked up in the modifier library. If an array of text or modifier objects are input here, different modifiers will be assigned based on cardinal direction, starting with north and moving clockwise. 

#### Outputs
* ##### hb_objs
The input honeybee objects with their modifiers edited. 