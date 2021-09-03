## CIE Standard Sky

![](../../images/components/CIE_Standard_Sky.png)

![](../../images/icons/CIE_Standard_Sky.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20CIE%20Standard%20Sky.py)


Create a point-in-time standard Radiance CIE sky. 



#### Inputs
* ##### north 
A number between 0 and 360 that represents the degrees off from the y-axis to make North. This can also be a vector to set the North. Default is 0. The default North direction is the Y-axis (0 degrees). 
* ##### location [Required]
A Ladybug location object. 
* ##### month 
An integer between 1 and 12 for the month of the year (default: 6). 
* ##### day 
An integer between 1 and 31 for the day of the month (default: 21). 
* ##### hour 
A number between 0 and 23.999 for the hour of the day (default: 12). 
* ##### type 
An integer between 0..5 to indicate CIE Sky Type (default: 0). 

    * 0 = Sunny with sun

    * 1 = sunny without sun

    * 2 = intermediate with sun

    * 3 = intermediate without sun

    * 4 = cloudy sky

    * 5 = uniform sky

#### Outputs
* ##### sky
A honeybee sky that can be used to create a point-in-time recipe. 