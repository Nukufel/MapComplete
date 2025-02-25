[//]: # (WARNING: this file is automatically generated. Please find the sources at the bottom and edit those sources)



 postoffices 
=============





A layer showing post offices.






  - This layer is shown at zoomlevel **12** and higher



## Table of contents

1. [ Themes using this layer ](#-themes-using-this-layer-)
2. [ Basic tags for this layer ](#-basic-tags-for-this-layer-)
3. [ Supported attributes ](#-supported-attributes-)
  - [just_created](#just_created)
  - [nothing_known](#nothing_known)
  - [images](#images)
  - [minimap](#minimap)
  - [opening_hours](#opening_hours)
  - [post_partner](#post_partner)
  - [post_offic_brand](#post_offic_brand)
  - [partner-brand](#partner-brand)
  - [letter-from](#letter-from)
  - [parcel-from](#parcel-from)
  - [parcel-pickup](#parcel-pickup)
  - [parcel-to](#parcel-to)
  - [stamps](#stamps)
  - [has_atm](#has_atm)
  - [leftover-questions](#leftover-questions)
  - [nearby_images](#nearby_images)
  - [lod](#lod)
  - [favourite_status](#favourite_status)
  - [share](#share)
  - [qr_code](#qr_code)
  - [last_edit](#last_edit)
  - [all-tags](#all-tags)
    + [Filters](#filters)

 Themes using this layer 
-------------------------





  - [atm](https://mapcomplete.org/atm)
  - [personal](https://mapcomplete.org/personal)
  - [postboxes](https://mapcomplete.org/postboxes)




 Basic tags for this layer 
---------------------------



Elements must match **any** of the following expressions:

 - <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dpost_office' target='_blank'>post_office</a>
 - <a href='https://wiki.openstreetmap.org/wiki/Key:post_office' target='_blank'>post_office</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office%3Dpost_partner' target='_blank'>post_partner</a>

[Execute on overpass](http://overpass-turbo.eu/?Q=%5Bout%3Ajson%5D%5Btimeout%3A90%5D%3B%28%20%20%20%20nwr%5B%22amenity%22%3D%22post_office%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%20%20%20%20nwr%5B%22post_office%22%3D%22post_partner%22%5D%28%7B%7Bbbox%7D%7D%29%3B%0A%29%3Bout%20body%3B%3E%3Bout%20skel%20qt%3B)



 Supported attributes 
----------------------



Warning: 

this quick overview is incomplete



attribute | type | values which are supported by this layer
----------- | ------ | ------------------------------------------
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/id#values) [id](https://wiki.openstreetmap.org/wiki/Key:id) | Multiple choice | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/opening_hours#values) [opening_hours](https://wiki.openstreetmap.org/wiki/Key:opening_hours) | [opening_hours](../SpecialInputElements.md#opening_hours) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/post_office#values) [post_office](https://wiki.openstreetmap.org/wiki/Key:post_office) | Multiple choice | [post_partner](https://wiki.openstreetmap.org/wiki/Tag:post_office%3Dpost_partner) [](https://wiki.openstreetmap.org/wiki/Tag:post_office%3D)
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/brand#values) [brand](https://wiki.openstreetmap.org/wiki/Key:brand) | [nsi](../SpecialInputElements.md#nsi) | 
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/post_office:brand#values) [post_office:brand](https://wiki.openstreetmap.org/wiki/Key:post_office:brand) | [string](../SpecialInputElements.md#string) | [DHL](https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DDHL) [DPD](https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DDPD) [GLS](https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DGLS) [UPS](https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DUPS) [DHL Paketshop](https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DDHL Paketshop) [Hermes PaketShop](https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DHermes PaketShop) [PostNL](https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DPostNL) [bpost](https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3Dbpost)
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/post_office:letter_from#values) [post_office:letter_from](https://wiki.openstreetmap.org/wiki/Key:post_office:letter_from) | [string](../SpecialInputElements.md#string) | [yes](https://wiki.openstreetmap.org/wiki/Tag:post_office:letter_from%3Dyes) [no](https://wiki.openstreetmap.org/wiki/Tag:post_office:letter_from%3Dno)
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/post_office:parcel_from#values) [post_office:parcel_from](https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_from) | [string](../SpecialInputElements.md#string) | [yes](https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_from%3Dyes) [no](https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_from%3Dno)
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/post_office:parcel_pickup#values) [post_office:parcel_pickup](https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_pickup) | [string](../SpecialInputElements.md#string) | [yes](https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_pickup%3Dyes) [no](https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_pickup%3Dno)
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/post_office:parcel_to#values) [post_office:parcel_to](https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_to) | [string](../SpecialInputElements.md#string) | [yes](https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_to%3Dyes) [no](https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_to%3Dno)
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/post_office:stamps#values) [post_office:stamps](https://wiki.openstreetmap.org/wiki/Key:post_office:stamps) | [string](../SpecialInputElements.md#string) | [yes](https://wiki.openstreetmap.org/wiki/Tag:post_office:stamps%3Dyes) [no](https://wiki.openstreetmap.org/wiki/Tag:post_office:stamps%3Dno)
[<img src='https://mapcomplete.org/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/atm#values) [atm](https://wiki.openstreetmap.org/wiki/Key:atm) | Multiple choice | [yes](https://wiki.openstreetmap.org/wiki/Tag:atm%3Dyes) [no](https://wiki.openstreetmap.org/wiki/Tag:atm%3Dno) [separate](https://wiki.openstreetmap.org/wiki/Tag:atm%3Dseparate)


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





### minimap

_This tagrendering has no question and is thus read-only_





### opening_hours

The question is `What are the opening hours for this post office?`
This rendering asks information about the property 
[opening_hours](https://wiki.openstreetmap.org/wiki/Key:opening_hours)
This is rendered with `<h3>Opening hours</h3>{opening_hours_table(opening_hours)}`
 -  *Marked as closed for an unspecified time* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:opening_hours' target='_blank'>opening_hours</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:opening_hours%3Dclosed' target='_blank'>closed</a>
 - _This option cannot be chosen as answer_



### post_partner

The question is `Is this a post partner?`

 -  *This shop is a post partner* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office' target='_blank'>post_office</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office%3Dpost_partner' target='_blank'>post_partner</a>
 -  *This shop is not a post partner* corresponds with post_office=



### post_offic_brand

The question is `To which brand does this post office belong?`
This rendering asks information about the property 
[brand](https://wiki.openstreetmap.org/wiki/Key:brand)
This is rendered with `This is a {brand} post office`

This tagrendering is only visible in the popup if the following condition is met: <a href='https://wiki.openstreetmap.org/wiki/Key:amenity' target='_blank'>amenity</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:amenity%3Dpost_office' target='_blank'>post_office</a>


### partner-brand

The question is `For which brand does this location offer services?`
This rendering asks information about the property 
[post_office:brand](https://wiki.openstreetmap.org/wiki/Key:post_office:brand)
This is rendered with `This location offers services for {post_office:brand}`
 -  *This location offers services for DHL* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:brand' target='_blank'>post_office:brand</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DDHL' target='_blank'>DHL</a>
 -  *This location offers services for DPD* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:brand' target='_blank'>post_office:brand</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DDPD' target='_blank'>DPD</a>
 -  *This location offers services for GLS* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:brand' target='_blank'>post_office:brand</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DGLS' target='_blank'>GLS</a>
 -  *This location offers services for UPS* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:brand' target='_blank'>post_office:brand</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DUPS' target='_blank'>UPS</a>
 -  *This location is a DHL Paketshop* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:brand' target='_blank'>post_office:brand</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DDHL Paketshop' target='_blank'>DHL Paketshop</a>
 -  *This location is a Hermes PaketShop* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:brand' target='_blank'>post_office:brand</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DHermes PaketShop' target='_blank'>Hermes PaketShop</a>
 -  *This location is a PostNL-point* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:brand' target='_blank'>post_office:brand</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3DPostNL' target='_blank'>PostNL</a>
 -  *This location offers services for bpost* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:brand' target='_blank'>post_office:brand</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:brand%3Dbpost' target='_blank'>bpost</a>
This tagrendering is only visible in the popup if the following condition is met: <a href='https://wiki.openstreetmap.org/wiki/Key:post_office' target='_blank'>post_office</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office%3Dpost_partner' target='_blank'>post_partner</a>


### letter-from

The question is `Can you post a letter here?`
This rendering asks information about the property 
[post_office:letter_from](https://wiki.openstreetmap.org/wiki/Key:post_office:letter_from)
This is rendered with `You can post letters with these companies: {post_office:letter_from}`
 -  *You can post letters here* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:letter_from' target='_blank'>post_office:letter_from</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:letter_from%3Dyes' target='_blank'>yes</a>
 -  *You can't post letters here* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:letter_from' target='_blank'>post_office:letter_from</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:letter_from%3Dno' target='_blank'>no</a>



### parcel-from

The question is `Can you send a parcel here?`
This rendering asks information about the property 
[post_office:parcel_from](https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_from)
This is rendered with `You can post parcels with these companies: {post_office:parcel_from}`
 -  *You can send parcels here* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_from' target='_blank'>post_office:parcel_from</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_from%3Dyes' target='_blank'>yes</a>
 -  *You can't send parcels here* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_from' target='_blank'>post_office:parcel_from</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_from%3Dno' target='_blank'>no</a>



### parcel-pickup

The question is `Can you pick up missed parcels here?`
This rendering asks information about the property 
[post_office:parcel_pickup](https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_pickup)
This is rendered with `You can pick up parcels from these companies: {post_office:parcel_pickup}`
 -  *You can pick up missed parcels here* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_pickup' target='_blank'>post_office:parcel_pickup</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_pickup%3Dyes' target='_blank'>yes</a>
 -  *You can't pick up missed parcels here* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_pickup' target='_blank'>post_office:parcel_pickup</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_pickup%3Dno' target='_blank'>no</a>



### parcel-to

The question is `Can you send parcels to here for pickup?`
This rendering asks information about the property 
[post_office:parcel_to](https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_to)
This is rendered with `You can send parcels to here for pickup with these companies: {post_office:parcel_to}`
 -  *You can send parcels to here for pickup* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_to' target='_blank'>post_office:parcel_to</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_to%3Dyes' target='_blank'>yes</a>
 -  *You can't send parcels to here for pickup* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:parcel_to' target='_blank'>post_office:parcel_to</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:parcel_to%3Dno' target='_blank'>no</a>



### stamps

The question is `Can you buy stamps here?`
This rendering asks information about the property 
[post_office:stamps](https://wiki.openstreetmap.org/wiki/Key:post_office:stamps)
This is rendered with `You can buy stamps from companies: {post_office:stamps}`
 -  *You can buy stamps here* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:stamps' target='_blank'>post_office:stamps</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:stamps%3Dyes' target='_blank'>yes</a>
 -  *You can't buy stamps here* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:post_office:stamps' target='_blank'>post_office:stamps</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:post_office:stamps%3Dno' target='_blank'>no</a>



### has_atm

The question is `Does this post office have an ATM?`

 -  *This post office has an ATM* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:atm' target='_blank'>atm</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:atm%3Dyes' target='_blank'>yes</a>
 -  *This post office does <b>not</b> have an ATM* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:atm' target='_blank'>atm</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:atm%3Dno' target='_blank'>no</a>
 -  *This post office does have an ATM, but it is mapped as a different icon* corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:atm' target='_blank'>atm</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:atm%3Dseparate' target='_blank'>separate</a>



### leftover-questions

_This tagrendering has no question and is thus read-only_





### nearby_images

_This tagrendering has no question and is thus read-only_



This tagrendering has labels 
`added_by_default_conditional`

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







#### Filters 





id | question | osmTags
---- | ---------- | ---------
open_now.0 | Open now | _isOpen=yes




id | question | osmTags
---- | ---------- | ---------
letter_from.0 | Offers letter posting | post_office:letter_from~.+ & post_office:letter_from!~^(no)$




id | question | osmTags
---- | ---------- | ---------
parcel_from.0 | Offers parcel posting | post_office:parcel_from~.+ & post_office:parcel_from!~^(no)$




id | question | osmTags
---- | ---------- | ---------
parcel_pickup.0 | Offers pickup of missed parcels | post_office:parcel_pickup~.+ & post_office:parcel_pickup!~^(no)$




id | question | osmTags
---- | ---------- | ---------
parcel_to.0 | Accepts pickup of parcels sent here | post_office:parcel_to~.+ & post_office:parcel_to!~^(no)$




id | question | osmTags
---- | ---------- | ---------
stamps.0 | Sells stamps | post_office:stamps~.+ & post_office:stamps!~^(no)$
 

This document is autogenerated from [assets/layers/postoffices/postoffices.json](https://github.com/pietervdvn/MapComplete/blob/develop/assets/layers/postoffices/postoffices.json)
