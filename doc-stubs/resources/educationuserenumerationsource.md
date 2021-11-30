---
title: "educationUserEnumerationSource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationUserEnumerationSource resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [educationEnumerationSource](../resources/educationenumerationsource.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|gradeLevelFilters|String collection|**TODO: Add Description** Inherited from [educationEnumerationSource](../resources/educationenumerationsource.md).|
|organizationFilters|String collection|**TODO: Add Description** Inherited from [educationEnumerationSource](../resources/educationenumerationsource.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleGroupsFilter|[roleGroup](../resources/rolegroup.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationUserEnumerationSource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationUserEnumerationSource",
  "organizationFilters": [
    "String"
  ],
  "gradeLevelFilters": [
    "String"
  ]
}
```

