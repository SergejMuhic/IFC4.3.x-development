Material Profile Set Usage
==========================

Material profile set usage defines layout at occurrences to indicate the offset from the 'Axis' reference curve according to cardinal point, and a reference extent such as for a default column height.

The material is defined by _IfcMaterialProfileSetUsage_ and is attached by the _IfcRelAssociatesMaterial_._RelatingMaterial_. It is accessible by the inverse _HasAssociations_ relationship. Elements with composite profiles can be represented by referring to several _IfcMaterialProfile_'s within the _IfcMaterialProfileSet_ that is referenced from the _IfcMaterialProfileSetUsage_.

```
concept {
    IfcProduct:HasAssociations -> IfcRelAssociatesMaterial:RelatedObjects
    IfcRelAssociatesMaterial:RelatingMaterial -> IfcMaterialProfileSetUsage
    IfcRelAssociatesMaterial:RelatingMaterial -> IfcMaterialProfileSetUsageTapering
    IfcMaterialProfileSetUsage:ForProfileSet -> IfcMaterialProfileSet_0
    IfcMaterialProfileSetUsage:CardinalPoint -> IfcCardinalPointReference_0
    IfcMaterialProfileSetUsage:ReferenceExtent -> IfcPositiveLengthMeasure
    IfcMaterialProfileSet_0:MaterialProfiles -> IfcMaterialProfile
    IfcMaterialProfileSet_0:MaterialProfiles -> IfcMaterialProfileWithOffsets
    IfcMaterialProfile:Material -> IfcMaterial
    IfcMaterialProfile:Profile -> IfcProfileDef
    IfcMaterial:HasRepresentation -> IfcMaterialDefinitionRepresentation:RepresentedMaterial
    IfcMaterialDefinitionRepresentation -> Material_Surface_Color_Style
    IfcMaterialProfileWithOffsets:OffsetValues -> IfcLengthMeasure
    IfcMaterialProfileSetUsageTapering:ForProfileEndSet -> IfcMaterialProfileSet_1
    IfcMaterialProfileSetUsageTapering:CardinalEndPoint -> IfcCardinalPointReference_1
    IfcMaterialProfile:Name[binding="Name"]
}
```
