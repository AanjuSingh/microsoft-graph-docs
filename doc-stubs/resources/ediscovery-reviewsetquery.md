---
title: "reviewSetQuery resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# reviewSetQuery resource type

Namespace: microsoft.graph.ediscovery



**TODO: Add Description**


Inherits from [entity](../resources/ediscovery-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List reviewSetQueries](../api/ediscovery-reviewsetquery-list.md)|[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) collection|Get a list of the [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) objects and their properties.|
|[Create reviewSetQuery](../api/ediscovery-reviewsetquery-create.md)|[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md)|Create a new [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.|
|[Get reviewSetQuery](../api/ediscovery-reviewsetquery-get.md)|[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md)|Read the properties and relationships of a [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.|
|[Update reviewSetQuery](../api/ediscovery-reviewsetquery-update.md)|[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md)|Update the properties of a [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.|
|[Delete reviewSetQuery](../api/ediscovery-reviewsetquery-delete.md)|None|Deletes a [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.|
|[applyTags](../api/ediscovery-reviewsetquery-applytags.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[microsoft.graph.identitySet](../resources/ediscovery-identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md).|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/ediscovery-identityset.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|query|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSetQuery",
  "id": "String (identifier)",
  "query": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

