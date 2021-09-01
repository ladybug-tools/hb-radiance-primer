# Annual Radiation Result

![](../../.gitbook/assets/Annual_Radiation_Result.png)

![](../../.gitbook/assets/Annual_Radiation_Result%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Annual%20Radiation%20Result.py)

Annual Daylight Metrics.

## Inputs

* **results \[Required\]**

  An list of annual Radiance result files from the "HB Annual Radiation" component.  This should include both the .ill files and the sun-up-hours.txt 

* **hoys**

  An optional integer or list of integers \(each greater than or equal to 0\) to select the hours of the year \(HOYs\) for which radiation results will be displayed. These HOYs can be obtained from the "LB Calculate HOY" or the "LB Analysis Period" components. If None, all hours of the results will be used. 

* **timestep**

  The timesteps per hour of the Wea that was used for the radiation analysis. This will be used to ensure radiation values are in the correct units. \(Default: 1\). 

## Outputs

* **report**

  Reports, errors, warnings, etc. 

* **irradiance**

  Average irradiance valules for each sensor in W/m2. 

* **radiation**

  Cumulative radiation valules for each sensor in Wh/m2. 

