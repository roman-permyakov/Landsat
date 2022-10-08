###### Landsat. Urban areas

# **Predicting Urban Areas with Machine Learning** <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/26/Landsat_Data_Continuity_Mission_Logo_%28transparent%29.png/120px-Landsat_Data_Continuity_Mission_Logo_%28transparent%29.png" height="50">
##  <p align="justify"> [Detect Urban Areas of Hyderabad in Landsat 5 imagery](https://yandex.ru/maps/20934/hyderabad/?from=tabbar&ll=78.429743%2C17.425630&mode=search&ol=geo&ouri=ymapsbm1%3A%2F%2Fgeo%3Fdata%3DCgoxNTUzMTkwNTQ4Ek1JbmRpYSwgU3RhdGUgb2YgVGVsYW5nYW5hLCBHcmVhdGVyIEh5ZGVyYWJhZCBNdW5pY2lwYWwgQ29ycG9yYXRpb24sIEh5ZGVyYWJhZCIKDTXqnEIVmzmLQQ%3D%3D&source=serp_navig&z=11.76)</p> 
 
###  Introduction

<p align="justify">The Landsat Thematic Mapper (TM) sensor was carried onboard Landsats 4 and 5 from July 1982 to May 2012 with
a 16-day repeat cycle. Landsat 4-5 TM image data files consist of seven spectral bands. The resolution is 30 meters for bands 1 to 7 
(thermal infrared band 6 was collected at 120 meters, but was resampled to 30 meters.) The approximate scene size is 170 km north-south
by 183 km east-west (106 mi by 114 mi).

Six bands (band 2 — band 7) of Landsat 5 TM are used as features to predict the binary built-up class.
A multispectral Landsat 5 data was acquired in 2011 for Bangalore, and its corresponding binary built-up layer will be used for
training and testing. Finally, another multispectral Landsat 5 data acquired in 2011 for Hyderabad will be used for new predictions.</p>

Google’s Tensorflow library is used in Python to build a Neural Network (NN).
The following other libraries will be required:

 * <b>pyrsgis</b> — to read and write GeoTIFF
 * <b>scikit-learn</b> — for data pre-processing and accuracy checks
 * <b>numpy</b> — for basic array operations
 * <b>Tensorflow</b> — to build the neural network model. </p>
 
 ### Content
 ```shell
 l5_Bangalore2011_raw.tif                - source training imagery
 l5_Bangalore2011_builtup.tif            - raster mask of buildings
 l5_Hyderabad2011_raw.tif.               - testing imagery
 Hyderabad_2011_BuiltupNN_predicted.tif  - raster mask of predicted buildings
  ```
<table>
<tr>
<td><img width="548" alt="image" src="https://user-images.githubusercontent.com/44007858/194723618-ced24b78-6fcf-426b-924c-ca02e8f9026a.png"></td>
<td><img width="549" alt="image" src="https://user-images.githubusercontent.com/44007858/194723631-6e43e2d9-2312-4ed0-b4f2-8a77e926a3c6.png"></td>
<td><img width="548" alt="image" src="https://user-images.githubusercontent.com/44007858/194723633-34b20c71-9113-41ca-9241-d8595a87591e.png"></td>
<td><img width="549" alt="image" src="https://user-images.githubusercontent.com/44007858/194723623-7121a573-25ce-4b23-b8cd-c0ca9fd39955.png"></td>
</tr>
</table> 

Inspired by [@PratyushTripathy](https://github.com/PratyushTripathy)
