---
title: "userExperienceAnalyticsOverview resource type"
description: "The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsOverview resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List userExperienceAnalyticsOverviews](../api/userexperienceanalyticsoverview-list.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) collection|Get a list of the [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) objects and their properties.|
|[Create userExperienceAnalyticsOverview](../api/userexperienceanalyticsoverview-create.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|Create a new [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[Get userExperienceAnalyticsOverview](../api/userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|Read the properties and relationships of a [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[Update userExperienceAnalyticsOverview](../api/userexperienceanalyticsoverview-update.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|Update the properties of a [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[Delete userExperienceAnalyticsOverview](../api/userexperienceanalyticsoverview-delete.md)|None|Deletes a [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appHealthOverallScore|Int32|The user experience analytics app health overall score.|
|appHealthState|userExperienceAnalyticsHealthState|The current health state of the user experience analytics 'BestPractices' category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|bestPracticesHealthState|userExperienceAnalyticsHealthState|The current health state of the user experience analytics 'BestPractices' category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|bestPracticesOverallScore|Int32|The user experience analytics best practices overall score.|
|deviceBootPerformanceHealthState|userExperienceAnalyticsHealthState|The current health state of the user experience analytics 'BootPerformance' category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|deviceBootPerformanceOverallScore|Int32|The user experience analytics device boot performance overall score.|
|id|String|The unique identifier of the user experience analytics overview.|
|insights|[userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection|The user experience analytics insights.|
|overallScore|Int32|The user experience analytics overall score.|
|resourcePerformanceHealthState|userExperienceAnalyticsHealthState|The current health state of the user experience analytics 'ResourcePerformance' category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|resourcePerformanceOverallScore|Int32|The user experience analytics resource performance overall score.|
|state|userExperienceAnalyticsHealthState|The current health state of the user experience analytics overview. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|workFromAnywhereHealthState|userExperienceAnalyticsHealthState|The current health state of the user experience analytics 'WorkFromAnywhere' category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|workFromAnywhereOverallScore|Int32|The user experience analytics Work From Anywhere overall score.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": "Integer",
  "deviceBootPerformanceOverallScore": "Integer",
  "bestPracticesOverallScore": "Integer",
  "workFromAnywhereOverallScore": "Integer",
  "appHealthOverallScore": "Integer",
  "resourcePerformanceOverallScore": "Integer",
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
    }
  ],
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String",
  "workFromAnywhereHealthState": "String",
  "appHealthState": "String",
  "resourcePerformanceHealthState": "String"
}
```

