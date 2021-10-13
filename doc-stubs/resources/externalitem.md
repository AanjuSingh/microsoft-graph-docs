---
title: "externalItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# externalItem resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List externalItems](../api/externalitem-list.md)|[externalItem](../resources/externalitem.md) collection|Get a list of the [externalItem](../resources/externalitem.md) objects and their properties.|
|[Create externalItem](../api/externalconnection-post-items.md)|[externalItem](../resources/externalitem.md)|Create a new [externalItem](../resources/externalitem.md) object.|
|[Get externalItem](../api/externalitem-get.md)|[externalItem](../resources/externalitem.md)|Read the properties and relationships of an [externalItem](../resources/externalitem.md) object.|
|[Update externalItem](../api/externalitem-update.md)|[externalItem](../resources/externalitem.md)|Update the properties of an [externalItem](../resources/externalitem.md) object.|
|[Delete externalItem](../api/externalitem-delete.md)|None|Deletes an [externalItem](../resources/externalitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acl|[acl](../resources/acl.md) collection|**TODO: Add Description**|
|content|[externalItemContent](../resources/externalitemcontent.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|properties|[properties](../resources/properties.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalItem",
  "id": "String (identifier)",
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl"
    }
  ],
  "content": {
    "@odata.type": "microsoft.graph.externalItemContent"
  },
  "properties": {
    "@odata.type": "microsoft.graph.properties"
  }
}
```

