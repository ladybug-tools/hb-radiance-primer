## BSModifier

![](../../images/components/BSModifier.png)

![](../../images/icons/BSModifier.png) - [[source code]](https://github.com/ladybug-tools/honeybee-grasshopper-radiance/blob/master/honeybee_grasshopper_radiance/src//HB%20BSDF%20Modifier.py)


Create a Bidirectional Scattering Distribution Function (BSDF) radiance modifier from an XML file. 



#### Inputs
* ##### xml_file [Required]
Path to an XML file contining BSDF data. These files can be produced using the LBNL WINDOW software among other sources. 
* ##### up_vec 
A vector that sets the hemisphere that the BSDF modifier faces. For materials that are symmetrical about the face plane (like non-angled venetian blinds), this can be any vector that is not perfectly normal/perpendicular to the face. For asymmetrica materials like angled venetian blinds, this variable should be coordinated with the direction that the geometry is facing. The default is set to (0.01, 0.01, 1.00), which should hopefully not be normal to any typical face. 
* ##### thickness 
Optional number to set the thickness of the BSDF. Thickness is not supported for aBSDF type. (Default: 0). 
* ##### bsdf_type 
An integer to set the bsdf type. Choose from the choices below. (Default: 0). 

    * 0 BSDF

    * 1 aBSDFChoose aBSDF (peak extraction) for systems with a strong specular transmission component. A proposed guideline for when to use aBSDF can be found in chapter 6 in "BSDF generation procedures for daylighting systems". Find the white paper at: 

    * https://task61.iea-shc.org/publications

#### Outputs
* ##### modifier
A BSDF modifier that can be assigned to a Honeybee geometry or Modifier Sets. 