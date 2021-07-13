---
title: "attendanceRecord resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# attendanceRecord resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attendanceIntervals|[attendanceInterval](../resources/attendanceinterval.md) collection|**TODO: Add Description**|
|emailAddress|String|**TODO: Add Description**|
|identity|[identity](../resources/identity.md)|**TODO: Add Description**|
|role|String|**TODO: Add Description**|
|totalAttendanceInSeconds|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attendanceRecord"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attendanceRecord",
  "attendanceIntervals": [
    {
      "@odata.type": "microsoft.graph.attendanceInterval"
    }
  ],
  "emailAddress": "String",
  "identity": {
    "@odata.type": "microsoft.graph.identity"
  },
  "role": "String",
  "totalAttendanceInSeconds": "Integer"
}
```

