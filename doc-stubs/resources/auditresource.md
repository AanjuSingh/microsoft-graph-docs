---
title: "auditResource resource type"
description: "A class containing the properties for Audit Resource."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# auditResource resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A class containing the properties for Audit Resource.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Display name.|
|modifiedProperties|[auditProperty](../resources/auditproperty.md) collection|List of modified properties.|
|resourceId|String|Audit resource's Id.|
|type|String|Audit resource's type.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty"
    }
  ],
  "resourceId": "String",
  "type": "String"
}
```

