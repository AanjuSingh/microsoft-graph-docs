---
title: "audioConferencing resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# audioConferencing resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|conferenceId|String|**TODO: Add Description**|
|dialinUrl|String|**TODO: Add Description**|
|tollFreeNumber|String|**TODO: Add Description**|
|tollFreeNumbers|String collection|**TODO: Add Description**|
|tollNumber|String|**TODO: Add Description**|
|tollNumbers|String collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.audioConferencing"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.audioConferencing",
  "conferenceId": "String",
  "dialinUrl": "String",
  "tollFreeNumber": "String",
  "tollFreeNumbers": [
    "String"
  ],
  "tollNumber": "String",
  "tollNumbers": [
    "String"
  ]
}
```

