---
title: "groupPrintUsageSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPrintUsageSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedJobCount|Int32|**TODO: Add Description**|
|group|[identity](../resources/identity.md)|**TODO: Add Description**|
|groupDisplayName|String|**TODO: Add Description**|
|groupMail|String|**TODO: Add Description**|
|incompleteJobCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPrintUsageSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPrintUsageSummary",
  "completedJobCount": "Integer",
  "group": {
    "@odata.type": "microsoft.graph.identity"
  },
  "groupDisplayName": "String",
  "groupMail": "String",
  "incompleteJobCount": "Integer"
}
```

