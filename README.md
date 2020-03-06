# ToolBox
An XML based framework, designed for making mod settings that allow changes to ThingDef properties. Examples: cost, hitpoints, beauty, etc. It can also be used to provide a guide or information regarding your mod. It currently has 10 property widgets that can be applied to a ThingDef, and will continue to expand in the future.

## Changelog
* Inital release [1.0.0.0]

## Table of content
* [Guide for Users](#Guide-for-Users)
  * [ThingDef Properties](#ThingDef-Properties)
* [Guide for Modders](#Guide-for-Modders)

## Guide for Users
### ThingDef Properties
Mods that uses ToolBox will have default ThingDef properties and is labeled based on what is it is. However, there may be instances when a mod has relabeled the widgets. Example: Fill is labeled as Cover. There are also varying update types to a property, such as Cost requiring a game restart while Beauty updates after change. Reload required changes are updated live, however, it will not function fully as intended. Reloading the save would fix those issues.

Properties | Description | Update Type
-----------|-------------|------------
Cost | amount of resources needed to construct. | Restart required
Beauty | rate of how enjoyable an object is to look at. | Live change
BaseHP | base MaxHP of an object, multiplied with the material. | Live change
Fill | percent of cover an object provides. | Live change
Path | reduction of movement to pass through an object. | Live change
Flammability | rate of how likely and strong an object burns. | Live change
Work | time it takes to build an object based on gameticks. 60 ticks is one second. | Live change
Passability | an object's state of being passable: Impassable, PassThroughOnly, or Standable. | Live change
Roof | an object's roofing mode: Auto, Manual, or None | Reload required
Link | type of link an object can connect to. There are 16 core linkFlags. | Reload required

### Guide for Modders
