---
title: "conditionalAccessUsers resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# conditionalAccessUsers resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|excludeGroups|String collection|**TODO: Add Description**|
|excludeGuestsOrExternalUsers|[conditionalAccessGuestsOrExternalUsers](../resources/conditionalaccessguestsorexternalusers.md)|**TODO: Add Description**|
|excludeRoles|String collection|**TODO: Add Description**|
|excludeUsers|String collection|**TODO: Add Description**|
|includeGroups|String collection|**TODO: Add Description**|
|includeGuestsOrExternalUsers|[conditionalAccessGuestsOrExternalUsers](../resources/conditionalaccessguestsorexternalusers.md)|**TODO: Add Description**|
|includeRoles|String collection|**TODO: Add Description**|
|includeUsers|String collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessUsers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conditionalAccessUsers",
  "excludeGroups": [
    "String"
  ],
  "excludeGuestsOrExternalUsers": {
    "@odata.type": "microsoft.graph.conditionalAccessGuestsOrExternalUsers"
  },
  "excludeRoles": [
    "String"
  ],
  "excludeUsers": [
    "String"
  ],
  "includeGroups": [
    "String"
  ],
  "includeGuestsOrExternalUsers": {
    "@odata.type": "microsoft.graph.conditionalAccessGuestsOrExternalUsers"
  },
  "includeRoles": [
    "String"
  ],
  "includeUsers": [
    "String"
  ]
}
```

