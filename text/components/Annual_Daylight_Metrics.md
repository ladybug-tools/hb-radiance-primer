## Annual Daylight Metrics

![](../../images/components/Annual_Daylight_Metrics.png)

![](../../images/icons/Annual_Daylight_Metrics.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Annual%20Daylight%20Metrics.py)


Annual Daylight Metrics. 



#### Inputs
* ##### results [Required]
An list of annual Radiance result files from the "HB Annual Daylight" component.  This should include both the .ill files and the sun-up-hours.txt 
* ##### occ_sch 
An annual occupancy schedule as a Ladybug Data Collection or a HB-Energy schedule object. This can also be the identifier of a schedule in your HB-Energy schedule library. Any value in this schedule that is 0.5 or above will be considered occupied. If None, a schedule from 9AM to 5PM on weekdays will be used. 
* ##### threshold 
Threshhold for daylight autonomy in lux (default: 300). 
* ##### min_max 
A list for min, max value for useful daylight illuminance 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### DA
Daylight autonomy. The percentage of time that each sensor recieves equal or more than the threshold. 
* ##### UDI
Useful daylight illuminance. The percentage of time that illuminace falls between minimum and maximum thresholds. 
* ##### UDI_low
Numbers for the percent of time that is below the lower threshold of useful daylight illuminance. 
* ##### UDI_up
Numbers for the percent of time that is above the upper threshold of useful daylight illuminance. 