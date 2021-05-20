## Deconstruct Wea

![](../../images/components/Deconstruct_Wea.png)

![](../../images/icons/Deconstruct_Wea.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Deconstruct%20Wea.py)


Deconstruct a Wea object into lists of direct, diffuse, and golbal radiation at each timestep of the file. 



#### Inputs
* ##### wea [Required]
A Honeybee WEA object. 

#### Outputs
* ##### dir
A list of direct normal irradiance values at each timestep of the WEA. 
* ##### diff
A list of diffuse sky solar irradiance values at each timestep of the WEA. 
* ##### glob
A list of global horizontal irradiance values at each timestep of the WEA. 