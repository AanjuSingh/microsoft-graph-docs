---
title: "managedDeviceSummarizedAppState resource type"
description: "Event representing a user's devices with failed or pending apps."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedDeviceSummarizedAppState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Event representing a user's devices with failed or pending apps.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceId|String|DeviceId of device represented by this object|
|summarizedAppState|runState|runState for the object. Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceSummarizedAppState",
  "deviceId": "String",
  "summarizedAppState": "String"
}
```

