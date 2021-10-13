---
title: "searchEntity resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# searchEntity resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get searchEntity](../api/searchentity-get.md)|[searchEntity](../resources/searchentity.md)|Read the properties and relationships of a [searchEntity](../resources/searchentity.md) object.|
|[Update searchEntity](../api/searchentity-update.md)|[searchEntity](../resources/searchentity.md)|Update the properties of a [searchEntity](../resources/searchentity.md) object.|
|[query](../api/searchentity-query.md)|[searchResponse](../resources/searchresponse.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|acronyms|[acronym](../resources/acronym.md) collection|**TODO: Add Description**|
|bookmarks|[bookmark](../resources/bookmark.md) collection|**TODO: Add Description**|
|qnas|[qna](../resources/qna.md) collection|**TODO: Add Description**|
|verticals|[vertical](../resources/vertical.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.searchEntity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.searchEntity",
  "id": "String (identifier)"
}
```

