---
title: "evaluateLabelJobResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# evaluateLabelJobResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|responsiblePolicy|[responsiblePolicy](../resources/responsiblepolicy.md)|**TODO: Add Description**|
|responsibleSensitiveTypes|[responsibleSensitiveType](../resources/responsiblesensitivetype.md) collection|**TODO: Add Description**|
|sensitivityLabel|[matchingLabel](../resources/matchinglabel.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.evaluateLabelJobResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.evaluateLabelJobResult",
  "responsiblePolicy": {
    "@odata.type": "microsoft.graph.responsiblePolicy"
  },
  "responsibleSensitiveTypes": [
    {
      "@odata.type": "microsoft.graph.responsibleSensitiveType"
    }
  ],
  "sensitivityLabel": {
    "@odata.type": "microsoft.graph.matchingLabel"
  }
}
```

