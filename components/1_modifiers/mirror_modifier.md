# Mirror Modifier

![](../../.gitbook/assets/Mirror_Modifier.png)

![](../../.gitbook/assets/Mirror_Modifier%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Mirror%20Modifier.py)

Create a mirror radiance modifier from a single reflectance.

## Inputs

* **name**

  Text to set the name for the modifier and to be incorporated into a unique modifier identifier. 

* **reflect \[Required\]**

  A number between 0 and 1 for the mirror reflectance. This reflectance will be the same for the red, green and blue channels. 

## Outputs

* **modifier**

  A mirror modifier that can be assigned to a Honeybee geometry or Modifier Sets. 

