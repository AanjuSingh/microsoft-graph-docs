---
title: "roleSuccessStatistics resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roleSuccessStatistics resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|permanentFail|Int64|**TODO: Add Description**|
|permanentSuccess|Int64|**TODO: Add Description**|
|removeFail|Int64|**TODO: Add Description**|
|removeSuccess|Int64|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|roleName|String|**TODO: Add Description**|
|temporaryFail|Int64|**TODO: Add Description**|
|temporarySuccess|Int64|**TODO: Add Description**|
|unknownFail|Int64|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleSuccessStatistics"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleSuccessStatistics",
  "permanentFail": "Integer",
  "permanentSuccess": "Integer",
  "removeFail": "Integer",
  "removeSuccess": "Integer",
  "roleId": "String",
  "roleName": "String",
  "temporaryFail": "Integer",
  "temporarySuccess": "Integer",
  "unknownFail": "Integer"
}
```

