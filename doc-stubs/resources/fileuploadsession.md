---
title: "fileUploadSession resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# fileUploadSession resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|containerExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|containerId|String|**TODO: Add Description**|
|sessionExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|sessionUri|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileUploadSession"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileUploadSession",
  "sessionUri": "String",
  "sessionExpirationDateTime": "String (timestamp)",
  "containerId": "String",
  "containerExpirationDateTime": "String (timestamp)"
}
```

