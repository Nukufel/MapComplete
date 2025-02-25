[//]: # (WARNING: this file is automatically generated. Please find the sources at the bottom and edit those sources)



 crab_address 
==============





Address data for Flanders by the governement, suited for import into OpenStreetMap. Datadump from 2021-10-26. This layer contains only visualisation logic. Import buttons should be added via an override. Note that HNRLABEL contains the original value, whereas _HNRLABEL contains a slightly cleaned version






  - This layer is shown at zoomlevel **0** and higher
  - <img src='../warning.svg' height='1rem'/> This layer is loaded from an external source, namely  `https://raw.githubusercontent.com/pietervdvn/MapComplete-data/main/CRAB_2021_10_26/tile_{z}_{x}_{y}.geojson`



## Table of contents

1. [ Themes using this layer ](#-themes-using-this-layer-)
2. [ Basic tags for this layer ](#-basic-tags-for-this-layer-)
3. [ Supported attributes ](#-supported-attributes-)
  - [just_created](#just_created)
  - [nothing_known](#nothing_known)
  - [render_crab](#render_crab)
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





  - [grb](https://mapcomplete.org/grb)




 Basic tags for this layer 
---------------------------



Elements must match the expression **HUISNR~.+**

[Execute on overpass](http://overpass-turbo.eu/?Q=%5Bout%3Ajson%5D%5Btimeout%3A90%5D%3B%28%20%20%20%20nwr%5B%22HUISNR%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%29%3Bout%20body%3B%3E%3Bout%20skel%20qt%3B)



 Supported attributes 
----------------------



Warning: 

this quick overview is incomplete



attribute | type | values which are supported by this layer
----------- | ------ | ------------------------------------------
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/id#values) [id](https://wiki.openstreetmap.org/wiki/Key:id) | Multiple choice | 


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

### render_crab

_This tagrendering has no question and is thus read-only_





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



 

This document is autogenerated from [assets/layers/crab_address/crab_address.json](https://github.com/pietervdvn/MapComplete/blob/develop/assets/layers/crab_address/crab_address.json)
