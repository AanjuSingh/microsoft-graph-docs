---
title: "operatingSystemVersionRange resource type"
description: "Operating System version range."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# operatingSystemVersionRange resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Operating System version range.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The description of this range (e.g. Valid 1702 builds)|
|highestVersion|String|The highest inclusive version that this range contains.|
|lowestVersion|String|The lowest inclusive version that this range contains.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "highestVersion": "String",
  "lowestVersion": "String"
}
```

