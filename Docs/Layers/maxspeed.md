[//]: # (WARNING: this file is automatically generated. Please find the sources at the bottom and edit those sources)



 maxspeed 
==========





Shows the allowed speed for every road






  - This layer is shown at zoomlevel **16** and higher



## Table of contents

1. [ Themes using this layer ](#-themes-using-this-layer-)
2. [ Basic tags for this layer ](#-basic-tags-for-this-layer-)
3. [ Supported attributes ](#-supported-attributes-)
  - [just_created](#just_created)
  - [nothing_known](#nothing_known)
  - [maxspeed-maxspeed](#maxspeed-maxspeed)
  - [leftover-questions](#leftover-questions)
  - [minimap](#minimap)
  - [split_button](#split_button)
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



Elements must match **all** of the following expressions:

0. <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dresidential' target='_blank'>residential</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dliving_street' target='_blank'>living_street</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dmotorway' target='_blank'>motorway</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dtertiary' target='_blank'>tertiary</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dunclassified' target='_blank'>unclassified</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dsecondary' target='_blank'>secondary</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dprimary' target='_blank'>primary</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dtrunk' target='_blank'>trunk</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dmotorway' target='_blank'>motorway</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dtertiary_link' target='_blank'>tertiary_link</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dsecondary_link' target='_blank'>secondary_link</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dprimary_link' target='_blank'>primary_link</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dtrunk_link' target='_blank'>trunk_link</a> | <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dmotorway_link' target='_blank'>motorway_link</a>
1. area!=yes
2. type!=multipolygon

[Execute on overpass](http://overpass-turbo.eu/?Q=%5Bout%3Ajson%5D%5Btimeout%3A90%5D%3B%28%20%20%20%20nwr%5B%22highway%22%3D%22residential%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22living_street%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22motorway%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22tertiary%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22unclassified%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22secondary%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22primary%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22trunk%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22motorway%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22tertiary_link%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22secondary_link%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22primary_link%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22trunk_link%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22highway%22%3D%22motorway_link%22%5D%5B%22area%22!%3D%22yes%22%5D%5B%22type%22!%3D%22multipolygon%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%29%3Bout%20body%3B%3E%3Bout%20skel%20qt%3B)



 Supported attributes 
----------------------



Warning: 

this quick overview is incomplete



attribute | type | values which are supported by this layer
----------- | ------ | ------------------------------------------
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/id#values) [id](https://wiki.openstreetmap.org/wiki/Key:id) | Multiple choice | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/maxspeed#values) [maxspeed](https://wiki.openstreetmap.org/wiki/Key:maxspeed) | [pnat](../SpecialInputElements.md#pnat) | 


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

### maxspeed-maxspeed

The question is `What is the legal maximum speed one is allowed to drive on this road?`
This rendering asks information about the property 
[maxspeed](https://wiki.openstreetmap.org/wiki/Key:maxspeed)
This is rendered with `The maximum allowed speed on this road is {canonical(maxspeed)}`
 - <img src='https://raw.githubusercontent.com/pietervdvn/MapComplete/develop/./assets/layers/maxspeed/living_street_be.svg' style='width: 3rem; height: 3rem'> *This is a living street, which has a maxspeed of 20km/h* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:highway' target='_blank'>highway</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:highway%3Dliving_street' target='_blank'>living_street</a> & <a href='https://wiki.openstreetmap.org/wiki/Key:_country' target='_blank'>_country</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:_country%3Dbe' target='_blank'>be</a>



### leftover-questions

_This tagrendering has no question and is thus read-only_





### minimap
Shows a small map with the feature. Added by default to every popup
_This tagrendering has no question and is thus read-only_





### split_button

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



 

This document is autogenerated from [assets/layers/maxspeed/maxspeed.json](https://github.com/pietervdvn/MapComplete/blob/develop/assets/layers/maxspeed/maxspeed.json)
