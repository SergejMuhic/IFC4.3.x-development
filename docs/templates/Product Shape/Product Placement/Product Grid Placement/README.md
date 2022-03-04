Product Grid Placement
======================

Product occurrences may be positioned relative to a grid, where the axes of such grid may be modified such that product occurrences are re-positioned relative to grid axes.

```
concept {
    IfcProduct:ObjectPlacement -> IfcGridPlacement
    IfcGridPlacement:PlacementLocation -> IfcVirtualGridIntersection
    IfcGridPlacement:PlacementRefDirection -> IfcDirection
    IfcGridPlacement:PlacementRelTo -> IfcObjectPlacement
    IfcVirtualGridIntersection:OffsetDistances -> IfcLengthMeasure_0
    IfcVirtualGridIntersection:IntersectingAxes -> IfcGridAxis
    IfcGridAxis:AxisTag -> IfcLabel
    IfcGridAxis:AxisCurve -> IfcLine
    IfcGridAxis:SameSense -> IfcBoolean
    IfcLine:Pnt -> IfcCartesianPoint
    IfcLine:Dir -> IfcVector
    IfcCartesianPoint:Coordinates -> IfcLengthMeasure_1
    IfcObjectPlacement:PlacesObject -> IfcGrid_0:ObjectPlacement
}
```
