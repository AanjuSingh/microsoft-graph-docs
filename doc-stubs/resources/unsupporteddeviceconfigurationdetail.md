---
title: "unsupportedDeviceConfigurationDetail resource type"
description: "A description of why an entity is unsupported."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# unsupportedDeviceConfigurationDetail resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A description of why an entity is unsupported.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|message|String|A message explaining why an entity is unsupported.|
|propertyName|String|If message is related to a specific property in the original entity, then the name of that property.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```

