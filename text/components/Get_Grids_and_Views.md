## Get Grids and Views

![](../../images/components/Get_Grids_and_Views.png)

![](../../images/icons/Get_Grids_and_Views.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Get%20Grids%20and%20Views.py)


Get Radiance Sensor Grids and/or Views from a Honeybee Model and visualize them in the Rhino scene. 



#### Inputs
* ##### model [Required]
A Honeybee Model for which grids and views will be output. 

#### Outputs
* ##### views
A list of Honeybee-Radiance Views that are assigned to the input _model. 
* ##### grids
A list of Honeybee-Radiance SensorGrids that are assigned to the input _model. 
* ##### points
The points that are at the center of each grid cell. 
* ##### meshes
Mesh for each sensor grid, which can be passed to the "LB Spatial Heatmap" component. 