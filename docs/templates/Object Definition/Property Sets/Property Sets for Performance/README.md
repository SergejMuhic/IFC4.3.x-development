Property Sets for Performance
=============================

For performance history, properties are in the form of time series, for tracking data at points in time.

```
concept {
    IfcObject:HasAssignments -> IfcRelAssignsToControl:RelatedObjects
    IfcRelAssignsToControl:RelatingControl -> IfcPerformanceHistory:Controls
    IfcPerformanceHistory:IsDefinedBy -> IfcRelDefinesByProperties:RelatedObjects
    IfcRelDefinesByProperties:RelatingPropertyDefinition -> IfcPropertySet
    IfcPropertySet:HasProperties -> IfcPropertyReferenceValue
    IfcPropertyReferenceValue:PropertyReference -> IfcRegularTimeSeries
    IfcRegularTimeSeries:Values -> IfcTimeSeriesValue
    IfcPropertyReferenceValue:PropertyReference -> IfcIrregularTimeSeries
    IfcIrregularTimeSeries:Values -> IfcIrregularTimeSeriesValue
    IfcIrregularTimeSeriesValue:TimeStamp -> IfcDateTime
    IfcIrregularTimeSeriesValue:ListValues -> IfcValue
}
```
