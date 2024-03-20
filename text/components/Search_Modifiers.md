## Search Modifiers

![](../../images/components/Search_Modifiers.png)

![](../../images/icons/Search_Modifiers.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20Search%20Modifiers.py)


Search for available Mofidiers within the honeybee standards library. 



#### Inputs
* ##### keywords 
Optional keywords to be used to narrow down the output list of modifiers. If nothing is input here, all available modifiers will be output. 
* ##### join_words 
If False or None, this component will automatically split any strings of multiple keywords (spearated by spaces) into separate keywords for searching. This results in a greater liklihood of finding an item in the search but it may not be appropropriate for all cases. You may want to set it to True when you are searching for a specific phrase that includes spaces. Default: False. 

#### Outputs
* ##### modifiers
A list of modifiers within the honeybee radiance standards library (filtered by keywords_ if they are input). 