# Apply Face Modifier

![](../../.gitbook/assets/Apply_Face_Modifier.png)

![](../../.gitbook/assets/Apply_Face_Modifier%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Apply%20Face%20Modifier.py)

Apply a Modifier to Honeybee Faces, Doors or Room walls.

This component supports the assigning of different modifiers based on cardinal orientation, provided that a list of Modifiers are input to the \_mod.

## Inputs

* **hb\_objs \[Required\]**

  Honeybee Faces, Doors or Rooms to which the input \_mod should be assigned. For the case of a Honeybee Room, the modifier will only be applied to the Room's outdoor walls. Note that, if you need to assign a modifier to all the roofs, floors, etc. of a Room, the best practice is to create a ModifierSet and assing that to the Room. 

* **mod \[Required\]**

  A Honeybee Modifier to be applied to the input \_hb\_objs. This can also be text for a modifier to be looked up in the modifier library. If an array of text or modifier objects are input here, different modifiers will be assigned based on cardinal direction, starting with north and moving clockwise. 

## Outputs

* **hb\_objs**

  The input honeybee objects with their modifiers edited. 

