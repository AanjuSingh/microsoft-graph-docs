---
title: "plannerUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# plannerUser resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [plannerDelta](../resources/plannerdelta.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List plannerUsers](../api/planneruser-list.md)|[plannerUser](../resources/planneruser.md) collection|Get a list of the [plannerUser](../resources/planneruser.md) objects and their properties.|
|[Create plannerUser](../api/planneruser-create.md)|[plannerUser](../resources/planneruser.md)|Create a new [plannerUser](../resources/planneruser.md) object.|
|[Get plannerUser](../api/planneruser-get.md)|[plannerUser](../resources/planneruser.md)|Read the properties and relationships of a [plannerUser](../resources/planneruser.md) object.|
|[Update plannerUser](../api/planneruser-update.md)|[plannerUser](../resources/planneruser.md)|Update the properties of a [plannerUser](../resources/planneruser.md) object.|
|[Delete plannerUser](../api/planneruser-delete.md)|None|Deletes a [plannerUser](../resources/planneruser.md) object.|
|[List all](../api/planneruser-list-all.md)|[plannerDelta](../resources/plannerdelta.md) collection|Get the plannerDelta resources from the all navigation property.|
|[Add plannerDelta](../api/planneruser-post-all.md)|[plannerDelta](../resources/plannerdelta.md)|Add all by posting to the all collection.|
|[List favoritePlans](../api/planneruser-list-favoriteplans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlan resources from the favoritePlans navigation property.|
|[Add plannerPlan](../api/planneruser-post-favoriteplans.md)|[plannerPlan](../resources/plannerplan.md)|Add favoritePlans by posting to the favoritePlans collection.|
|[List plans](../api/planneruser-list-plans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlan resources from the plans navigation property.|
|[Add plannerPlan](../api/planneruser-post-plans.md)|[plannerPlan](../resources/plannerplan.md)|Add plans by posting to the plans collection.|
|[List recentPlans](../api/planneruser-list-recentplans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlan resources from the recentPlans navigation property.|
|[Add plannerPlan](../api/planneruser-post-recentplans.md)|[plannerPlan](../resources/plannerplan.md)|Add recentPlans by posting to the recentPlans collection.|
|[List rosterPlans](../api/planneruser-list-rosterplans.md)|[plannerPlan](../resources/plannerplan.md) collection|Get the plannerPlan resources from the rosterPlans navigation property.|
|[Add plannerPlan](../api/planneruser-post-rosterplans.md)|[plannerPlan](../resources/plannerplan.md)|Add rosterPlans by posting to the rosterPlans collection.|
|[List tasks](../api/planneruser-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTask resources from the tasks navigation property.|
|[Add plannerTask](../api/planneruser-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Add tasks by posting to the tasks collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](../resources/plannerfavoriteplanreferencecollection.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](../resources/plannerrecentplanreferencecollection.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|all|[plannerDelta](../resources/plannerdelta.md) collection|**TODO: Add Description**|
|favoritePlans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|
|plans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|
|recentPlans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|
|rosterPlans|[plannerPlan](../resources/plannerplan.md) collection|**TODO: Add Description**|
|tasks|[plannerTask](../resources/plannertask.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerUser",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerUser",
  "id": "String (identifier)",
  "favoritePlanReferences": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
  },
  "recentPlanReferences": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
  }
}
```

