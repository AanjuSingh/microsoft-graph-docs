---
title: "connectionOperation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# connectionOperation resource type

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/externalconnectors-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List connectionOperations](../api/externalconnectors-connectionoperation-list.md)|[microsoft.graph.externalConnectors.connectionOperation](../resources/externalconnectors-connectionoperation.md) collection|Get a list of the [connectionOperation](../resources/externalconnectors-connectionoperation.md) objects and their properties.|
|[Create connectionOperation](../api/externalconnectors-connectionoperation-create.md)|[microsoft.graph.externalConnectors.connectionOperation](../resources/externalconnectors-connectionoperation.md)|Create a new [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.|
|[Get connectionOperation](../api/externalconnectors-connectionoperation-get.md)|[microsoft.graph.externalConnectors.connectionOperation](../resources/externalconnectors-connectionoperation.md)|Read the properties and relationships of a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.|
|[Update connectionOperation](../api/externalconnectors-connectionoperation-update.md)|[microsoft.graph.externalConnectors.connectionOperation](../resources/externalconnectors-connectionoperation.md)|Update the properties of a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.|
|[Delete connectionOperation](../api/externalconnectors-connectionoperation-delete.md)|None|Deletes a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[microsoft.graph.publicError](../resources/externalconnectors-publicerror.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/externalconnectors-entity.md).|
|status|connectionOperationStatus|**TODO: Add Description**. Possible values are: `unspecified`, `inprogress`, `completed`, `failed`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalConnectors.connectionOperation",
  "id": "String (identifier)",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "status": "String"
}
```

