## Daylight Factor

![](../../images/components/Daylight_Factor.png)

![](../../images/icons/Daylight_Factor.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Daylight%20Factor.py)


Run a daylight factor study for a Honeybee model. 

Daylight Factor (DF) is defined as the ratio of the indoor daylight illuminance to outdoor illuminance under an unobstructed overcast sky. It is expressed as a percentage between 0 and 100. 

Because daylight factor is computed using an overcast sky, it does not change with [North, East, South, West] orientation. As such, it is more suited to assessing daylight in climates where cloudy conditions are common. The "HB Annual Daylight" recipe yields a much more accurate assessment of daylight and is suitable for all climates, though it requires a significantly longer calculation time than Daylight Factor. 



#### Inputs
* ##### model [Required]
A Honeybee Model for which Daylight Factor will be simulated. Note that this model should have grids assigned to it in order to produce meaningfule results. 
* ##### grid_filter 
Text for a grid identifer or a pattern to filter the sensor grids of the model that are simulated. For instance, `first_floor_*` will simulate only the sensor grids that have an identifier that starts with `first_floor_`. By default, all grids in the model will be simulated. 
* ##### sensor_count 
Integer for the maximum number of sensor grid points per parallel execution. (Default: 200). 
* ##### radiance_par 
Text for the radiance parameters to be used for ray tracing. (Default: -ab 2 -aa 0.1 -ad 2048 -ar 64). 
* ##### run_settings 
Settings from the "HB Recipe Settings" component that specify how the recipe should be run. This can also be a text string of recipe settings. 
* ##### run [Required]
Set to True to run the recipe and get results. This input can also be the integer "2" to run the recipe silently. 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### results
The daylight factor values from the simulation in percent. Each value is for a different sensor of the grid. These can be plugged into the "LB Spatial Heatmap" component along with meshes of the sensor grids to visualize results. 