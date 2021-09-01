# Glass Modifier

![](../../.gitbook/assets/Glass_Modifier.png)

![](../../.gitbook/assets/Glass_Modifier%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Glass%20Modifier.py)

Create an glass radiance modifier from a single transmittance.

## Inputs

* **name**

  Text to set the name for the modifier and to be incorporated into a unique modifier identifier. 

* **trans \[Required\]**

  A number between 0 and 1 for the glass modifier transmittance. This transmittance will be the same for the red, green and blue channels. 

* **refract**

  Index of refraction. Typical values are 1.52 for float glass and 1.4 for ETFE. If None, Radiance will default to using 1.52 for glass \(Default: None\). 

## Outputs

* **modifier**

  A glass modifier that can be assigned to a Honeybee geometry or Modifier Sets. 

