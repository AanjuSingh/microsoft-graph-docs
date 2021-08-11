---
title: "userExperienceAnalyticsMetric resource type"
description: "The user experience analytics metric contains the score and units of a metric of a user experience anlaytics category."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsMetric resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics metric contains the score and units of a metric of a user experience anlaytics category.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List userExperienceAnalyticsMetrics](../api/userexperienceanalyticsmetric-list.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) collection|Get a list of the [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) objects and their properties.|
|[Create userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-create.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Create a new [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[Get userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-get.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Read the properties and relationships of a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[Update userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-update.md)|[userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md)|Update the properties of a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|
|[Delete userExperienceAnalyticsMetric](../api/userexperienceanalyticsmetric-delete.md)|None|Deletes a [userExperienceAnalyticsMetric](../resources/userexperienceanalyticsmetric.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier of the user experience analytics metric.|
|unit|String|The unit of the user experience analytics metric.|
|value|Double|The value of the user experience analytics metric.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsMetric",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsMetric",
  "id": "String (identifier)",
  "value": "Double",
  "unit": "String"
}
```

