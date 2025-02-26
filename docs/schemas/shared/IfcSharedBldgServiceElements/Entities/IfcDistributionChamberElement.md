# IfcDistributionChamberElement

A distribution chamber element defines a place at which distribution systems and their constituent elements may be inspected or through which they may travel.

An **IfcDistributionChamberElement** is a formed volume used in a distribution system, such as a sump, trench or manhole. Instances of IfcDistributionSystem or IfcDistributionFlowElement may be related to the **IfcDistributionChamberElement** enabling their location in or at the chamber to be determined.

> HISTORY  New entity in IFC2x2.

## Attributes

### PredefinedType


## Formal Propositions

### CorrectPredefinedType


### CorrectTypeAssigned

## Concepts

### Material Constituent Set

The material of the **IfcDistributionChamberElement** is defined by [IfcMaterialConstituentSet](../../ifcmaterialresource/lexical/ifcmaterialconstituentset.htm) or as a fallback by [IfcMaterial](../../ifcmaterialresource/lexical/ifcmaterial.htm), and attached by the RelatingMaterial attribute on the [IfcRelAssociatesMaterial](../../ifcproductextension/lexical/ifcrelassociatesmaterial.htm) relationship. It is accessible by the HasAssociations inverse attribute. Material information can also be given at the [IfcDistributionChamberElementType](../../ifcsharedbldgserviceelements/lexical/ifcdistributionchamberelementtype.htm), defining the common attribute data for all occurrences of the same type. The following keywords for _IfcMaterialConstituentSet.MaterialConstituents[n].Name_ shall be used:

* **'Base'**: The material from which the base of the duct is constructed.
* **'Cover'**: The material from which the access cover to the chamber is constructed.
* **'Fill'**: The material that is used to fill the duct (where used).
* **'Wall'**: The material from which the wall of the duct is constructed.

#### Base

The material from which the base of the duct is constructed.

#### Cover

The material from which the access cover to the chamber is constructed.

#### Fill

The material that is  used to fill the duct (where used).

#### Wall

The material from which the wall of the duct is constructed.

### Object Typing



### Property Sets for Objects



### Quantity Sets



