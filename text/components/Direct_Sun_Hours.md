## Direct Sun Hours

![](../../images/components/Direct_Sun_Hours.png)

![](../../images/icons/Direct_Sun_Hours.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Direct%20Sun%20Hours.py)


Calculate the number of hours of direct sun received by grids of sensors in a Honeybee model. 



#### Inputs
* ##### model [Required]
A Honeybee Model for which Direct Sun Hours will be simulated. Note that this model should have grids assigned to it in order to produce meaningfule results. 
* ##### wea [Required]
A Wea object produced from the Wea components that are under the Light Sources tab. This can also be the path to a .wea or a .epw file. 
* ##### north 
A number between -360 and 360 for the counterclockwise difference between the North and the positive Y-axis in degrees. This can also be Vector for the direction to North. (Default: 0). 
* ##### grid_filter 
Text for a grid identifer or a pattern to filter the sensor grids of the model that are simulated. For instance, first_floor_* will simulate only the sensor grids that have an identifier that starts with first_floor_. By default, all grids in the model will be simulated. 
* ##### sensor_count 
Integer for the maximum number of sensor grid points per parallel execution. (Default: 200). 
* ##### run_settings 
Settings from the "HB Recipe Settings" component that specify how the recipe should be run. This can also be a text string of recipe settings. 
* ##### run [Required]
Set to True to run the recipe and get results. 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### results
Folder with raw result files (.ill) that contain the number of timesteps that each sensor is exposed to sun. The units are the timestep of input wea file. For an hourly wea, each value corresponds to an hour of direct sun. 
* ##### hours
The cumulative number of timesteps that each sensor sees the sun. If the input wea timestep is 1, the results are the number of direct sun hours. 