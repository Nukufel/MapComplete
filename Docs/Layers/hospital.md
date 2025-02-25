[//]: # (WARNING: this file is automatically generated. Please find the sources at the bottom and edit those sources)



 hospital 
==========





A layer showing hospital grounds






  - This layer is shown at zoomlevel **12** and higher



## Table of contents

1. [ Themes using this layer ](#-themes-using-this-layer-)
2. [ Basic tags for this layer ](#-basic-tags-for-this-layer-)
3. [ Supported attributes ](#-supported-attributes-)
  - [just_created](#just_created)
  - [nothing_known](#nothing_known)
  - [name](#name)
  - [inpatient](#inpatient)
  - [phone](#phone)
  - [email](#email)
  - [website](#website)
  - [oh-visitor](#oh-visitor)
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





  - [disaster_response](https://mapcomplete.org/disaster_response)
  - [healthcare](https://mapcomplete.org/healthcare)
  - [onwheels](https://mapcomplete.org/onwheels)
  - [personal](https://mapcomplete.org/personal)




 Basic tags for this layer 
---------------------------



Elements must match **any** of the following expressions:

 - <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dhospital' target='_blank'>hospital</a>
 - <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dclinic' target='_blank'>clinic</a>

[Execute on overpass](http://overpass-turbo.eu/?Q=%5Bout%3Ajson%5D%5Btimeout%3A90%5D%3B%28%20%20%20%20nwr%5B%22amenity%22%3D%22hospital%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22amenity%22%3D%22clinic%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%29%3Bout%20body%3B%3E%3Bout%20skel%20qt%3B)



 Supported attributes 
----------------------



Warning: 

this quick overview is incomplete



attribute | type | values which are supported by this layer
----------- | ------ | ------------------------------------------
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/id#values) [id](https://wiki.openstreetmap.org/wiki/Key:id) | Multiple choice | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/name#values) [name](https://wiki.openstreetmap.org/wiki/Key:name) | [string](../SpecialInputElements.md#string) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/amenity#values) [amenity](https://wiki.openstreetmap.org/wiki/Key:amenity) | Multiple choice | [clinic](https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dclinic) [hospital](https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dhospital)
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/phone#values) [phone](https://wiki.openstreetmap.org/wiki/Key:phone) | [phone](../SpecialInputElements.md#phone) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/email#values) [email](https://wiki.openstreetmap.org/wiki/Key:email) | [email](../SpecialInputElements.md#email) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/website#values) [website](https://wiki.openstreetmap.org/wiki/Key:website) | [url](../SpecialInputElements.md#url) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/opening_hours:visitors#values) [opening_hours:visitors](https://wiki.openstreetmap.org/wiki/Key:opening_hours:visitors) | [opening_hours](../SpecialInputElements.md#opening_hours) | 


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

The question is `What is the name of this hospital?`
This rendering asks information about the property 
[name](https://wiki.openstreetmap.org/wiki/Key:name)
This is rendered with `This hospital is called {name}`




### inpatient

The question is `Does this facility admit inpatients?`

 -  *This is a clinic - patients can not stay overnight* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dclinic' target='_blank'>clinic</a>
 -  *This is a hospital - patients can be admitted here for multiple days* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dhospital' target='_blank'>hospital</a>



### phone

The question is `What is the phone number of {title()}?`
This rendering asks information about the property 
[phone](https://wiki.openstreetmap.org/wiki/Key:phone)
This is rendered with `<a href='tel:{phone}'>{phone}</a>`
 - <img src='https://raw.githubusercontent.com/pietervdvn/MapComplete/develop/./assets/layers/questions/phone.svg' style='width: 3rem; height: 3rem'> *<a href='tel:{contact:phone}'>{contact:phone}</a>* corresponds with contact:phone~.+
 - _This option cannot be chosen as answer_

This tagrendering has labels 
`contact`

### email

The question is `What is the email address of {title()}?`
This rendering asks information about the property 
[email](https://wiki.openstreetmap.org/wiki/Key:email)
This is rendered with `<a href='mailto:{email}' target='_blank' rel='noopener'>{email}</a>`
 - <img src='https://raw.githubusercontent.com/pietervdvn/MapComplete/develop/./assets/svg/envelope.svg' style='width: 3rem; height: 3rem'> *<a href='mailto:{contact:email}' target='_blank' rel='noopener'>{contact:email}</a>* corresponds with contact:email~.+
 - _This option cannot be chosen as answer_
 - <img src='https://raw.githubusercontent.com/pietervdvn/MapComplete/develop/./assets/svg/envelope.svg' style='width: 3rem; height: 3rem'> *<a href='mailto:{operator:email}' target='_blank' rel='noopener'>{operator:email}</a>* corresponds with operator:email~.+
 - _This option cannot be chosen as answer_

This tagrendering has labels 
`contact`

### website

The question is `What is the website of {title()}?`
This rendering asks information about the property 
[website](https://wiki.openstreetmap.org/wiki/Key:website)
This is rendered with `<a href='{website}' rel='nofollow noopener noreferrer' target='_blank'>{website}</a>`
 - <img src='https://raw.githubusercontent.com/pietervdvn/MapComplete/develop/./assets/layers/icons/website.svg' style='width: 3rem; height: 3rem'> *<a href='{contact:website}' rel='nofollow noopener noreferrer' target='_blank'>{contact:website}</a>* corresponds with contact:website~.+
 - _This option cannot be chosen as answer_

This tagrendering has labels 
`contact`

### oh-visitor

The question is `When are visitors allowed to visit?`
This rendering asks information about the property 
[opening_hours:visitors](https://wiki.openstreetmap.org/wiki/Key:opening_hours:visitors)
This is rendered with `<h3>Opening hours for visitors</h3>Regular visitors are allowed at the following moments: {opening_hours_table(opening_hours:visitors)}<p class='subtle'>Some wands might have different opening hours. Many hospitals allow visits during emergencies too.</p>`




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



 

This document is autogenerated from [assets/layers/hospital/hospital.json](https://github.com/pietervdvn/MapComplete/blob/develop/assets/layers/hospital/hospital.json)
