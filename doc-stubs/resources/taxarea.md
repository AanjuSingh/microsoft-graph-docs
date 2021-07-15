---
title: "taxArea resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# taxArea resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List taxAreas](../api/taxarea-list.md)|[taxArea](../resources/taxarea.md) collection|Get a list of the [taxArea](../resources/taxarea.md) objects and their properties.|
|[Create taxArea](../api/taxarea-create.md)|[taxArea](../resources/taxarea.md)|Create a new [taxArea](../resources/taxarea.md) object.|
|[Get taxArea](../api/taxarea-get.md)|[taxArea](../resources/taxarea.md)|Read the properties and relationships of a [taxArea](../resources/taxarea.md) object.|
|[Update taxArea](../api/taxarea-update.md)|[taxArea](../resources/taxarea.md)|Update the properties of a [taxArea](../resources/taxarea.md) object.|
|[Delete taxArea](../api/taxarea-delete.md)|None|Deletes a [taxArea](../resources/taxarea.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|taxType|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taxArea",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taxArea",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "taxType": "String"
}
```

