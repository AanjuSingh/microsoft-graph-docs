---
title: "hasPayloadLinkResultItem resource type"
description: "A class containing the result of HasPayloadLinks action."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# hasPayloadLinkResultItem resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A class containing the result of HasPayloadLinks action.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|String|Exception information indicates if check for this item was successful or not.Empty string for no error.|
|hasLink|Boolean|Indicate whether a payload has any link or not.|
|payloadId|String|Key of the Payload, In the format of Guid.|
|sources|deviceAndAppManagementAssignmentSource collection|The reason where the link comes from.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hasPayloadLinkResultItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hasPayloadLinkResultItem",
  "error": "String",
  "hasLink": "Boolean",
  "payloadId": "String",
  "sources": [
    "String"
  ]
}
```

