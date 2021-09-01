# Sensor Grid

![](../../.gitbook/assets/Sensor_Grid.png)

![](../../.gitbook/assets/Sensor_Grid%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Sensor%20Grid.py)

Create a Sensor Grid object that can be used in a grid-based recipe.

## Inputs

* **name**

  A name for this sensor grid. 

* **positions \[Required\]**

  A list or a datatree of points with one point for the position of eah sensor. Each branch of the datatree will be considered as a separate sensor grid. 

* **directions**

  A list or a datatree of vectors with one vector for the direction of each sensor. The input here MUST therefor align with the input \_positions. If no value is provided \(0, 0, 1\) will be assigned for all the sensors. 

* **mesh**

  An optional mesh that aligns with the sensors. This is useful for generating visualizations of the sensor grid beyond the sensor positions. Note that the number of sensors in the grid must match the number of faces or the number vertices within the mesh. 

* **base\_geo**

  An optional Brep for the geometry used to make the grid. There are no restrictions on how this brep relates to the sensors and it is provided only to assist with the display of the grid when the number of sensors or the mesh is too large to be practically visualized. 

## Outputs

* **grid**

  An SensorGrid object that can be used in a grid-based recipe. 

