

 observation_tower 
===================



<img src='https://mapcomplete.osm.be/./assets/layers/observation_tower/Tower_observation.svg' height="100px"> 

Towers with a panoramic view




## Table of contents

1. [observation_tower](#observation_tower)
      * [Themes using this layer](#themes-using-this-layer)
  - [Basic tags for this layer](#basic-tags-for-this-layer)
  - [Supported attributes](#supported-attributes)
    + [images](#images)
    + [name](#name)
    + [Height](#height)
    + [Operator](#operator)
    + [website](#website)
    + [Fee](#fee)
    + [payment-options](#payment-options)
    + [wheelchair-access](#wheelchair-access)
    + [wikipedia](#wikipedia)










#### Themes using this layer 





  - [observation_towers](https://mapcomplete.osm.be/observation_towers)


[Go to the source code](../assets/layers/observation_tower/observation_tower.json)



 Basic tags for this layer 
---------------------------



Elements must have the all of following tags to be shown on this layer:



  - <a href='https://wiki.openstreetmap.org/wiki/Key:tower:type' target='_blank'>tower:type</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:tower:type%3Dobservation' target='_blank'>observation</a>




 Supported attributes 
----------------------



**Warning** This quick overview is incomplete



attribute | type | values which are supported by this layer
----------- | ------ | ------------------------------------------
[<img src='https://mapcomplete.osm.be/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/name#values) [name](https://wiki.openstreetmap.org/wiki/Key:name) | [string](../SpecialInputElements.md#string) | 
[<img src='https://mapcomplete.osm.be/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/height#values) [height](https://wiki.openstreetmap.org/wiki/Key:height) | [pfloat](../SpecialInputElements.md#pfloat) | 
[<img src='https://mapcomplete.osm.be/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/operator#values) [operator](https://wiki.openstreetmap.org/wiki/Key:operator) | [string](../SpecialInputElements.md#string) | 
[<img src='https://mapcomplete.osm.be/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/website#values) [website](https://wiki.openstreetmap.org/wiki/Key:website) | [url](../SpecialInputElements.md#url) | 
[<img src='https://mapcomplete.osm.be/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/charge#values) [charge](https://wiki.openstreetmap.org/wiki/Key:charge) | [string](../SpecialInputElements.md#string) | [](https://wiki.openstreetmap.org/wiki/Tag:charge%3D)
[<img src='https://mapcomplete.osm.be/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/wheelchair#values) [wheelchair](https://wiki.openstreetmap.org/wiki/Key:wheelchair) | Multiple choice | [designated](https://wiki.openstreetmap.org/wiki/Tag:wheelchair%3Ddesignated) [yes](https://wiki.openstreetmap.org/wiki/Tag:wheelchair%3Dyes) [limited](https://wiki.openstreetmap.org/wiki/Tag:wheelchair%3Dlimited) [no](https://wiki.openstreetmap.org/wiki/Tag:wheelchair%3Dno)
[<img src='https://mapcomplete.osm.be/assets/svg/statistics.svg' height='18px'>](https://taginfo.openstreetmap.org/keys/wikidata#values) [wikidata](https://wiki.openstreetmap.org/wiki/Key:wikidata) | [wikidata](../SpecialInputElements.md#wikidata) | 




### images 



_This tagrendering has no question and is thus read-only_





### name 



The question is **What is the name of this tower?**

This rendering asks information about the property  [name](https://wiki.openstreetmap.org/wiki/Key:name) 
This is rendered with `This tower is called <b>{name}</b>`



  - **This tower doesn't have a specific name** corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:noname' target='_blank'>noname</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:noname%3Dyes' target='_blank'>yes</a>




### Height 



The question is **What is the height of this tower?**

This rendering asks information about the property  [height](https://wiki.openstreetmap.org/wiki/Key:height) 
This is rendered with `This tower is {height} high`



### Operator 



The question is **Who maintains this tower?**

This rendering asks information about the property  [operator](https://wiki.openstreetmap.org/wiki/Key:operator) 
This is rendered with `Maintained by <b>{operator}</b>`



### website 



The question is **What is the website of {name}?**

This rendering asks information about the property  [website](https://wiki.openstreetmap.org/wiki/Key:website) 
This is rendered with `<a href='{website}' target='_blank'>{website}</a>`



  - **<a href='{contact:website}' target='_blank'>{contact:website}</a>** corresponds with contact:website~^..*$_This option cannot be chosen as answer_




### Fee 



The question is **How much does one have to pay to enter this tower?**

This rendering asks information about the property  [charge](https://wiki.openstreetmap.org/wiki/Key:charge) 
This is rendered with `Visiting this tower costs <b>{charge}</b>`



  - **Free to visit** corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:fee' target='_blank'>fee</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:fee%3Dno' target='_blank'>no</a>




### payment-options 



The question is **Which methods of payment are accepted here?**





  - **Cash is accepted here** corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:payment:cash' target='_blank'>payment:cash</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:payment:cash%3Dyes' target='_blank'>yes</a>Unselecting this answer will add <a href='https://wiki.openstreetmap.org/wiki/Key:payment:cash' target='_blank'>payment:cash</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:payment:cash%3Dno' target='_blank'>no</a>
  - **Payment cards are accepted here** corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:payment:cards' target='_blank'>payment:cards</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:payment:cards%3Dyes' target='_blank'>yes</a>Unselecting this answer will add <a href='https://wiki.openstreetmap.org/wiki/Key:payment:cards' target='_blank'>payment:cards</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:payment:cards%3Dno' target='_blank'>no</a>




### wheelchair-access 



The question is **Is this place accessible with a wheelchair?**





  - **This place is specially adapted for wheelchair users** corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:wheelchair' target='_blank'>wheelchair</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:wheelchair%3Ddesignated' target='_blank'>designated</a>
  - **This place is easily reachable with a wheelchair** corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:wheelchair' target='_blank'>wheelchair</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:wheelchair%3Dyes' target='_blank'>yes</a>
  - **It is possible to reach this place in a wheelchair, but it is not easy** corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:wheelchair' target='_blank'>wheelchair</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:wheelchair%3Dlimited' target='_blank'>limited</a>
  - **This place is not reachable with a wheelchair** corresponds with <a href='https://wiki.openstreetmap.org/wiki/Key:wheelchair' target='_blank'>wheelchair</a>=<a href='https://wiki.openstreetmap.org/wiki/Tag:wheelchair%3Dno' target='_blank'>no</a>




### wikipedia 



The question is **What is the corresponding Wikidata entity?**

This rendering asks information about the property  [wikidata](https://wiki.openstreetmap.org/wiki/Key:wikidata) 
This is rendered with `{wikipedia():max-height:25rem}`



  - **No Wikipedia page has been linked yet** corresponds with _This option cannot be chosen as answer_
 

This document is autogenerated from assets/layers/observation_tower/observation_tower.json