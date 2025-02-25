[//]: # (WARNING: this file is automatically generated. Please find the sources at the bottom and edit those sources)



 speed_display 
===============





Layer showing speed displays that alert drivers of their speed.






  - This layer is shown at zoomlevel **12** and higher



## Table of contents

1. [ Themes using this layer ](#-themes-using-this-layer-)
2. [ Basic tags for this layer ](#-basic-tags-for-this-layer-)
3. [ Supported attributes ](#-supported-attributes-)
  - [just_created](#just_created)
  - [nothing_known](#nothing_known)
  - [maxspeed](#maxspeed)
  - [inscription](#inscription)
  - [leftover-questions](#leftover-questions)
  - [minimap](#minimap)
  - [lod](#lod)
  - [favourite_status](#favourite_status)
  - [share](#share)
  - [qr_code](#qr_code)
  - [last_edit](#last_edit)
  - [all-tags](#all-tags)

 Themes using this layer 
-------------------------





  - [maxspeed](https://mapcomplete.org/maxspeed)
  - [personal](https://mapcomplete.org/personal)




 Basic tags for this layer 
---------------------------



Elements must match the expression **<a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dspeed_display' target='_blank'>speed_display</a>**

[Execute on overpass](http://overpass-turbo.eu/?Q=%5Bout%3Ajson%5D%5Btimeout%3A90%5D%3B%28%20%20%20%20nwr%5B%22highway%22%3D%22speed_display%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%29%3Bout%20body%3B%3E%3Bout%20skel%20qt%3B)



 Supported attributes 
----------------------



Warning: 

this quick overview is incomplete



attribute | type | values which are supported by this layer
----------- | ------ | ------------------------------------------
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/id#values) [id](https://wiki.openstreetmap.org/wiki/Key:id) | Multiple choice | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/maxspeed#values) [maxspeed](https://wiki.openstreetmap.org/wiki/Key:maxspeed) | [pnat](../SpecialInputElements.md#pnat) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/inscription#values) [inscription](https://wiki.openstreetmap.org/wiki/Key:inscription) | [string](../SpecialInputElements.md#string) | 


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

### maxspeed

The question is `What is the maximum speed allowed at this speed display?`
This rendering asks information about the property 
[maxspeed](https://wiki.openstreetmap.org/wiki/Key:maxspeed)
This is rendered with `The maximum speed allowed at this speed display is {canonical(maxspeed)}`




### inscription

The question is `What is the text on this speed display?`
This rendering asks information about the property 
[inscription](https://wiki.openstreetmap.org/wiki/Key:inscription)
This is rendered with `The text on this speed display is {inscription}`




### leftover-questions

_This tagrendering has no question and is thus read-only_





### minimap
Shows a small map with the feature. Added by default to every popup
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



 

This document is autogenerated from [assets/layers/speed_display/speed_display.json](https://github.com/pietervdvn/MapComplete/blob/develop/assets/layers/speed_display/speed_display.json)
