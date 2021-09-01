# Annual Radiation

![](../../.gitbook/assets/Annual_Radiation.png)

![](../../.gitbook/assets/Annual_Radiation%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Annual%20Radiation.py)

Run an annual radiation study for a Honeybee model.

The annual radiation values will be for each timestep of the input wea file.

Total radiation is calculated by summing together the direct irradiance from sun disks and the contribution from indirect sky radiation.

## Inputs

* **model \[Required\]**

  A Honeybee Model for which Annual Radiation will be simulated. Note that this model should have grids assigned to it in order to produce meaningfule results. 

* **wea \[Required\]**

  A Wea object produced from the Wea components that are under the Light Sources tab. This can also be the path to a .wea or a .epw file. 

* **north**

  A number between -360 and 360 for the counterclockwise difference between the North and the positive Y-axis in degrees. This can also be Vector for the direction to North. \(Default: 0\). 

* **grid\_filter**

  Text for a grid identifer or a pattern to filter the sensor grids of the model that are simulated. For instance, first_floor_\* will simulate only the sensor grids that have an identifier that starts with first_floor_. By default, all grids in the model will be simulated. 

* **sensor\_count**

  Integer for the maximum number of sensor grid points per parallel execution. \(Default: 200\). 

* **radiance\_par**

  Text for the radiance parameters to be used for ray tracing. \(Default: -ab 2 -ad 5000 -lw 2e-05\). 

* **run\_settings**

  Settings from the "HB Recipe Settings" component that specify how the recipe should be run. This can also be a text string of recipe settings. 

* **run \[Required\]**

  Set to True to run the recipe and get results. 

## Outputs

* **report**

  Reports, errors, warnings, etc. 

* **total**

  Folder with raw result files \(.ill\) that contain irradiance matrices for the total radiation at each sensor and timestep. 

* **direct**

  Folder with raw result files \(.ill\) that contain irradiance matrices for the direct radiation at each sensor and timestep. 

