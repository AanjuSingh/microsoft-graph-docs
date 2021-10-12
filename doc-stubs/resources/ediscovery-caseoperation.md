---
title: "caseOperation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# caseOperation resource type

Namespace: microsoft.graph.ediscovery



**TODO: Add Description**


Inherits from [entity](../resources/ediscovery-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List caseOperations](../api/ediscovery-caseoperation-list.md)|[microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) collection|Get a list of the [caseOperation](../resources/ediscovery-caseoperation.md) objects and their properties.|
|[Create caseOperation](../api/ediscovery-caseoperation-create.md)|[microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md)|Create a new [caseOperation](../resources/ediscovery-caseoperation.md) object.|
|[Get caseOperation](../api/ediscovery-caseoperation-get.md)|[microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md)|Read the properties and relationships of a [caseOperation](../resources/ediscovery-caseoperation.md) object.|
|[Update caseOperation](../api/ediscovery-caseoperation-update.md)|[microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md)|Update the properties of a [caseOperation](../resources/ediscovery-caseoperation.md) object.|
|[Delete caseOperation](../api/ediscovery-caseoperation-delete.md)|None|Deletes a [caseOperation](../resources/ediscovery-caseoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|caseAction|**TODO: Add Description**. The possible values are: `contentExport`, `applyTags`, `convertToPdf`, `index`, `estimateStatistics`, `addToReviewSet`, `unknownFutureValue`.|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|createdBy|[microsoft.graph.identitySet](../resources/ediscovery-identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md).|
|percentProgress|Int32|**TODO: Add Description**|
|resultInfo|[microsoft.graph.resultInfo](../resources/ediscovery-resultinfo.md)|**TODO: Add Description**|
|status|caseOperationStatus|**TODO: Add Description**. The possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```

