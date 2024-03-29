## Annual Average Values

![](../../images/components/Annual_Average_Values.png)

![](../../images/icons/Annual_Average_Values.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Annual%20Average%20Values.py)


Get average illuminance or irradiance values over an annual daylight or irradiance simulation. 

The _hoys_ input can also be used to filter the data for a particular time period or hour/timestep of the simulation. 



#### Inputs
* ##### results [Required]
An list of annual Radiance result files from either the "HB Annual Daylight" or the "HB Annual Irradiance" component (containing the .ill files and the sun-up-hours.txt). This can also be just the path to the folder containing these result files. 
* ##### dyn_sch 
Optional dynamic Aperture Group Schedules from the "HB Aperture Group Schedule" component, which will be used to customize the behavior of any dyanmic aperture geometry in the output metrics. If unsupplied, all dynamic aperture groups will be in their default state in for the output metrics. 
* ##### hoys 
An optional numbers or list of numbers to select the hours of the year (HOYs) for which results will be computed. These HOYs can be obtained from the "LB Calculate HOY" or the "LB Analysis Period" components. If None, all hours of the results will be used. 
* ##### median 
Set to True to get the median values instead of the average. The median values can only be calculated for a results folder from the "HB Annual Daylight" component. (Default: False). 
* ##### grid_filter 
The name of a grid or a pattern to filter the grids. For instance, first_floor_* will simulate only the sensor grids that have an identifier that starts with first_floor_. By default all the grids will be processed. 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### values
Average illuminance or irradiance valules for each sensor in lux or W/m2. Each value is for a different sensor of the grid. These can be plugged into the "LB Spatial Heatmap" component along with meshes of the sensor grids to visualize results. 