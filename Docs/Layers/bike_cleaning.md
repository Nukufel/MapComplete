[//]: # (WARNING: this file is automatically generated. Please find the sources at the bottom and edit those sources)



 bike_cleaning 
===============





A layer showing facilities where one can clean their bike






  - This layer is shown at zoomlevel **13** and higher



## Table of contents

1. [ Themes using this layer ](#-themes-using-this-layer-)
2. [ Basic tags for this layer ](#-basic-tags-for-this-layer-)
3. [ Supported attributes ](#-supported-attributes-)
  - [just_created](#just_created)
  - [nothing_known](#nothing_known)
  - [images](#images)
  - [bike_cleaning-service:bicycle:cleaning:charge](#bike_cleaning-servicebicycle:cleaning:charge)
  - [bike_cleaning-charge](#bike_cleaning-charge)
  - [leftover-questions](#leftover-questions)
  - [minimap](#minimap)
  - [nearby_images](#nearby_images)
  - [move-button](#move-button)
  - [delete-button](#delete-button)
  - [lod](#lod)
  - [favourite_status](#favourite_status)
  - [share](#share)
  - [qr_code](#qr_code)
  - [last_edit](#last_edit)
  - [all-tags](#all-tags)

 Themes using this layer 
-------------------------





  - [cyclofix](https://mapcomplete.org/cyclofix)
  - [personal](https://mapcomplete.org/personal)




 Basic tags for this layer 
---------------------------



Elements must match **any** of the following expressions:

 - <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dbicycle_wash' target='_blank'>bicycle_wash</a>
 - <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dbike_wash' target='_blank'>bike_wash</a>
 - <a href='https://wiki.openstreetmap.org/wiki/Key:service:bicycle:cleaning' target='_blank'>service:bicycle:cleaning</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:service:bicycle:cleaning%3Dyes' target='_blank'>yes</a>
 - <a href='https://wiki.openstreetmap.org/wiki/Key:service:bicycle:cleaning' target='_blank'>service:bicycle:cleaning</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:service:bicycle:cleaning%3Ddiy' target='_blank'>diy</a>

[Execute on overpass](http://overpass-turbo.eu/?Q=%5Bout%3Ajson%5D%5Btimeout%3A90%5D%3B%28%20%20%20%20nwr%5B%22amenity%22%3D%22bicycle_wash%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22amenity%22%3D%22bike_wash%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22service%3Abicycle%3Acleaning%22%3D%22yes%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22service%3Abicycle%3Acleaning%22%3D%22diy%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%29%3Bout%20body%3B%3E%3Bout%20skel%20qt%3B)



 Supported attributes 
----------------------



Warning: 

this quick overview is incomplete



attribute | type | values which are supported by this layer
----------- | ------ | ------------------------------------------
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/id#values) [id](https://wiki.openstreetmap.org/wiki/Key:id) | Multiple choice | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/service:bicycle:cleaning:charge#values) [service:bicycle:cleaning:charge](https://wiki.openstreetmap.org/wiki/Key:service:bicycle:cleaning:charge) | [string](../SpecialInputElements.md#string) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/charge#values) [charge](https://wiki.openstreetmap.org/wiki/Key:charge) | [string](../SpecialInputElements.md#string) | 


### just_created
This element shows a 'thank you' that the contributor has recently created this element
_This tagrendering has no question and is thus read-only_

 - <img src='https://raw.githubusercontent.com/pietervdvn/MapComplete/develop/./assets/svg/party.svg' style='width: 3rem; height: 3rem'> *You just created this element! Thanks for sharing this info with the world and helping people worldwide.* corresponds with id~.+
This tagrendering is only visible in the popup if the following condition is met: _last_edit:passed_time<300 & (_version_number= | <a href='https://wiki.openstreetmap.org/wiki/Key:_version_number' target='_blank'>_version_number</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:_version_number%3D1' target='_blank'>1</a>) & _backend~.+
This tagrendering has labels 
`added_by_default_top`

### nothing_known

_This tagrendering has no question and is thus read-only_


This tagrendering is only visible in the popup if the following condition is met: _last_edit:passed_time>=300 & _backend~.+
This tagrendering has labels 
`added_by_default_top`

### images
This block shows the known images which are linked with the `image`-keys, but also via `mapillary` and `wikidata` and shows the button to upload new images
_This tagrendering has no question and is thus read-only_





### bike_cleaning-service:bicycle:cleaning:charge

The question is `How much does it cost to use the cleaning service?`
This rendering asks information about the property 
[service:bicycle:cleaning:charge](https://wiki.openstreetmap.org/wiki/Key:service:bicycle:cleaning:charge)
This is rendered with `Using the cleaning service costs {service:bicycle:cleaning:charge}`
 -  *The cleaning service is free to use* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:service:bicycle:cleaning:fee' target='_blank'>service:bicycle:cleaning:fee</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:service:bicycle:cleaning:fee%3Dno' target='_blank'>no</a>
 -  *Free to use* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:service:bicycle:cleaning:fee' target='_blank'>service:bicycle:cleaning:fee</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:service:bicycle:cleaning:fee%3Dyes' target='_blank'>yes</a> & service:bicycle:cleaning:charge=
 - _This option cannot be chosen as answer_
This tagrendering is only visible in the popup if the following condition is met: amenity!=bike_wash & amenity!=bicycle_wash & service:bicycle:cleaning!=no & service:bicycle:cleaning~.+


### bike_cleaning-charge

The question is `How much does it cost to use the cleaning service?`
This rendering asks information about the property 
[charge](https://wiki.openstreetmap.org/wiki/Key:charge)
This is rendered with `Using the cleaning service costs {charge}`
 -  *This cleaning service is free to use* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:fee' target='_blank'>fee</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:fee%3Dno' target='_blank'>no</a>
 -  *There is a fee to use this cleaning service* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:fee' target='_blank'>fee</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:fee%3Dyes' target='_blank'>yes</a>
This tagrendering is only visible in the popup if the following condition is met: <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dbike_wash' target='_blank'>bike_wash</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dbicycle_wash' target='_blank'>bicycle_wash</a>


### leftover-questions

_This tagrendering has no question and is thus read-only_





### minimap
Shows a small map with the feature. Added by default to every popup
_This tagrendering has no question and is thus read-only_





### nearby_images

_This tagrendering has no question and is thus read-only_



This tagrendering has labels 
`added_by_default_conditional`

### move-button

_This tagrendering has no question and is thus read-only_





### delete-button

_This tagrendering has no question and is thus read-only_





### lod

_This tagrendering has no question and is thus read-only_



This tagrendering has labels 
`added_by_default`

### favourite_status

_This tagrendering has no question and is thus read-only_



This tagrendering has labels 
`added_by_default`

### share

_This tagrendering has no question and is thus read-only_



This tagrendering has labels 
`added_by_default`

### qr_code

_This tagrendering has no question and is thus read-only_



This tagrendering has labels 
`added_by_default`

### last_edit
Gives some metainfo about the last edit and who did edit it - rendering only
_This tagrendering has no question and is thus read-only_


This tagrendering is only visible in the popup if the following condition is met: _last_edit:changeset~.+ & _last_edit:contributor~.+
This tagrendering has labels 
`added_by_default`

### all-tags

_This tagrendering has no question and is thus read-only_



 

This document is autogenerated from [assets/layers/bike_cleaning/bike_cleaning.json](https://github.com/pietervdvn/MapComplete/blob/develop/assets/layers/bike_cleaning/bike_cleaning.json)
