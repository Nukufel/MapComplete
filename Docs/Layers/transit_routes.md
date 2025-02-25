[//]: # (WARNING: this file is automatically generated. Please find the sources at the bottom and edit those sources)



 transit_routes 
================





Layer showing bus lines






  - This layer is shown at zoomlevel **15** and higher
  - Not rendered on the map by default. If you want to rendering this on the map, override `mapRenderings`



## Table of contents

1. [ Themes using this layer ](#-themes-using-this-layer-)
2. [ Basic tags for this layer ](#-basic-tags-for-this-layer-)
3. [ Supported attributes ](#-supported-attributes-)
  - [just_created](#just_created)
  - [nothing_known](#nothing_known)
  - [name](#name)
  - [from](#from)
  - [via](#via)
  - [to](#to)
  - [colour](#colour)
  - [network](#network)
  - [operator](#operator)
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





  - [personal](https://mapcomplete.org/personal)
  - [transit](https://mapcomplete.org/transit)




 Basic tags for this layer 
---------------------------



Elements must match **all** of the following expressions:

0. <a href='https://wiki.openstreetmap.org/wiki/Key:route' target='_blank'>route</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:route%3Dbus' target='_blank'>bus</a>
1. <a href='https://wiki.openstreetmap.org/wiki/Key:type' target='_blank'>type</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:type%3Droute' target='_blank'>route</a>

[Execute on overpass](http://overpass-turbo.eu/?Q=%5Bout%3Ajson%5D%5Btimeout%3A90%5D%3B%28%20%20%20%20nwr%5B%22route%22%3D%22bus%22%5D%5B%22type%22%3D%22route%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%29%3Bout%20body%3B%3E%3Bout%20skel%20qt%3B)



 Supported attributes 
----------------------



Warning: 

this quick overview is incomplete



attribute | type | values which are supported by this layer
----------- | ------ | ------------------------------------------
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/id#values) [id](https://wiki.openstreetmap.org/wiki/Key:id) | Multiple choice | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/name#values) [name](https://wiki.openstreetmap.org/wiki/Key:name) | [string](../SpecialInputElements.md#string) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/from#values) [from](https://wiki.openstreetmap.org/wiki/Key:from) | [string](../SpecialInputElements.md#string) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/via#values) [via](https://wiki.openstreetmap.org/wiki/Key:via) | [string](../SpecialInputElements.md#string) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/to#values) [to](https://wiki.openstreetmap.org/wiki/Key:to) | [string](../SpecialInputElements.md#string) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/colour#values) [colour](https://wiki.openstreetmap.org/wiki/Key:colour) | [color](../SpecialInputElements.md#color) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/network#values) [network](https://wiki.openstreetmap.org/wiki/Key:network) | [string](../SpecialInputElements.md#string) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/operator#values) [operator](https://wiki.openstreetmap.org/wiki/Key:operator) | [string](../SpecialInputElements.md#string) | 


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

### name

The question is `What is the name for this bus line? (i.e. Bus XX: From => Via => To)`
This rendering asks information about the property 
[name](https://wiki.openstreetmap.org/wiki/Key:name)
This is rendered with `{name}`




### from

The question is `What is the starting point for this bus line?`
This rendering asks information about the property 
[from](https://wiki.openstreetmap.org/wiki/Key:from)
This is rendered with `This bus line begins at {from}`




### via

The question is `What is the via point for this bus line?`
This rendering asks information about the property 
[via](https://wiki.openstreetmap.org/wiki/Key:via)
This is rendered with `This bus line goes via {via}`




### to

The question is `What is the ending point for this bus line?`
This rendering asks information about the property 
[to](https://wiki.openstreetmap.org/wiki/Key:to)
This is rendered with `This bus line ends at {to}`




### colour

The question is `What is the colour for this bus line?`
This rendering asks information about the property 
[colour](https://wiki.openstreetmap.org/wiki/Key:colour)
This is rendered with `This bus line has the color {colour}`




### network

The question is `What network does this bus line belong to?`
This rendering asks information about the property 
[network](https://wiki.openstreetmap.org/wiki/Key:network)
This is rendered with `This bus line is part of the {network} network`




### operator

The question is `What company operates this bus line?`
This rendering asks information about the property 
[operator](https://wiki.openstreetmap.org/wiki/Key:operator)
This is rendered with `This bus line is operated by {operator}`




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



 

This document is autogenerated from [assets/layers/transit_routes/transit_routes.json](https://github.com/pietervdvn/MapComplete/blob/develop/assets/layers/transit_routes/transit_routes.json)
