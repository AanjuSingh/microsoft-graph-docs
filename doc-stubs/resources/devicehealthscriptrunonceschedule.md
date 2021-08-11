---
title: "deviceHealthScriptRunOnceSchedule resource type"
description: "Device health script run once schedule."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptRunOnceSchedule resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device health script run once schedule.


Inherits from [deviceHealthScriptTimeSchedule](../resources/devicehealthscripttimeschedule.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|date|Date|The date the script is scheduled to run. This collection can contain a maximum of 20 elements.|
|interval|Int32|The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule. Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/devicehealthscriptrunschedule.md).|
|time|TimeOfDay|At what time the script is scheduled to run. This collection can contain a maximum of 20 elements. Inherited from [deviceHealthScriptTimeSchedule](../resources/devicehealthscripttimeschedule.md).|
|useUtc|Boolean|Indicate if the time is Utc or client local time. Inherited from [deviceHealthScriptTimeSchedule](../resources/devicehealthscripttimeschedule.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunOnceSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunOnceSchedule",
  "interval": "Integer",
  "useUtc": "Boolean",
  "time": "String (time of day)",
  "date": "Date"
}
```

