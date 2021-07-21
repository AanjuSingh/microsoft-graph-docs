---
title: "plannerPlanDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# plannerPlanDetails resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [plannerDelta](../resources/plannerdelta.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List plannerPlanDetails](../api/plannerplandetails-list.md)|[plannerPlanDetails](../resources/plannerplandetails.md) collection|Get a list of the [plannerPlanDetails](../resources/plannerplandetails.md) objects and their properties.|
|[Create plannerPlanDetails](../api/plannerplandetails-create.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Create a new [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Read the properties and relationships of a [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[Update plannerPlanDetails](../api/plannerplandetails-update.md)|[plannerPlanDetails](../resources/plannerplandetails.md)|Update the properties of a [plannerPlanDetails](../resources/plannerplandetails.md) object.|
|[Delete plannerPlanDetails](../api/plannerplandetails-delete.md)|None|Deletes a [plannerPlanDetails](../resources/plannerplandetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|categoryDescriptions|[plannerCategoryDescriptions](../resources/plannercategorydescriptions.md)|**TODO: Add Description**|
|contextDetails|[plannerPlanContextDetailsCollection](../resources/plannerplancontextdetailscollection.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|sharedWith|[plannerUserIds](../resources/planneruserids.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerPlanDetails",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "id": "String (identifier)",
  "categoryDescriptions": {
    "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
  },
  "contextDetails": {
    "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
  },
  "sharedWith": {
    "@odata.type": "microsoft.graph.plannerUserIds"
  }
}
```

