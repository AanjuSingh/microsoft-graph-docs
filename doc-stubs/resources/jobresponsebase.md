---
title: "jobResponseBase resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# jobResponseBase resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List jobResponseBases](../api/jobresponsebase-list.md)|[jobResponseBase](../resources/jobresponsebase.md) collection|Get a list of the [jobResponseBase](../resources/jobresponsebase.md) objects and their properties.|
|[Create jobResponseBase](../api/jobresponsebase-create.md)|[jobResponseBase](../resources/jobresponsebase.md)|Create a new [jobResponseBase](../resources/jobresponsebase.md) object.|
|[Get jobResponseBase](../api/jobresponsebase-get.md)|[jobResponseBase](../resources/jobresponsebase.md)|Read the properties and relationships of a [jobResponseBase](../resources/jobresponsebase.md) object.|
|[Update jobResponseBase](../api/jobresponsebase-update.md)|[jobResponseBase](../resources/jobresponsebase.md)|Update the properties of a [jobResponseBase](../resources/jobresponsebase.md) object.|
|[Delete jobResponseBase](../api/jobresponsebase-delete.md)|None|Deletes a [jobResponseBase](../resources/jobresponsebase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|error|[classificationError](../resources/classificationerror.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.jobResponseBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "id": "String (identifier)",
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError"
  },
  "startDateTime": "String (timestamp)",
  "status": "String",
  "tenantId": "String",
  "type": "String"
}
```

